<template>
  <el-input-number v-model="num1" />
  <el-input-number v-model="num2" size="medium" />
  <el-input-number v-model="num3" size="small" />
  <el-input-number v-model="num4" size="mini" />
  <el-input-number
      v-model="num"
      :min="1"
      :max="10"
      controls-position="right"
  />
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup() {
    const num = ref(1)
    const num1 = ref(1)
    const num2 = ref(2)
    const num3 = ref(3)
    const num4 = ref(4)
    return {
      num,
      num1,
      num2,
      num3,
      num4,
    }
  },
})
</script>
