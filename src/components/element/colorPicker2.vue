<template>
  <div class="demo-color-sizes">
    <el-color-picker v-model="color" />
    <el-color-picker v-model="color" size="medium" />
    <el-color-picker v-model="color" size="small" />
    <el-color-picker v-model="color" size="mini" />
    <el-color-picker v-model="color" show-alpha :predefine="predefineColors" />
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup() {
    const color = ref('409EFF')

    const predefineColors = ref([
      '#ff4500',
      '#ff8c00',
      '#ffd700',
      '#90ee90',
      '#00ced1',
      '#1e90ff',
      '#c71585',
      'rgba(255, 69, 0, 0.68)',
      'rgb(255, 120, 0)',
      'hsv(51, 100, 98)',
      'hsva(120, 40, 94, 0.5)',
      'hsl(181, 100%, 37%)',
      'hsla(209, 100%, 56%, 0.73)',
      '#c7158577',
    ])

    return {
      color,
      predefineColors
    }
  },
})
</script>

<style lang="scss">
.demo-color-sizes {
  .el-color-picker:not(:last-child) {
    margin-right: 16px;
  }
}
</style>
