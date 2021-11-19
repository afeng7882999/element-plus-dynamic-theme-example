<template>
  <div class="demo-image__preview">
    <el-image
        style="width: 100px; height: 100px"
        :src="url"
        :preview-src-list="srcList"
    >
    </el-image>
  </div>
  <div class="demo-image__error">
    <div class="block">
      <span class="demonstration">Default</span>
      <el-image></el-image>
    </div>
    <div class="block">
      <span class="demonstration">Custom</span>
      <el-image>
        <template #error>
          <div class="image-slot">
            <el-icon><picture /></el-icon>
          </div>
        </template>
      </el-image>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
import { Picture } from '@element-plus/icons'

export default defineComponent({
  setup() {
    const url = ref(
        'https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg'
    )
    const srcList = ref([
      'https://fuss10.elemecdn.com/8/27/f01c15bb73e1ef3793e64e6b7bbccjpeg.jpeg',
      'https://fuss10.elemecdn.com/1/8e/aeffeb4de74e2fde4bd74fc7b4486jpeg.jpeg',
    ])

    return {
      url,
      srcList,
    }
  },
})
</script>
