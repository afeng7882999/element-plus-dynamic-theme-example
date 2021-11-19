<template>
  <el-radio-group v-model="state.themeName" @change="onRadioGroupChanged">
    <el-radio label="默认">默认</el-radio>
    <el-radio label="火焰">火焰</el-radio>
    <el-radio label="暗黑">暗黑</el-radio>
    <el-radio label="军旅">军旅</el-radio>
    <el-radio label="糖果">糖果</el-radio>
  </el-radio-group>
</template>

<script setup lang="ts">
  import {reactive} from "vue";
  import {themeProcess, setDocumentTheme, CUSTOM_THEME, DEFAULT_THEMES, Theme} from "element-plus-dynamic-theme/theme";

  const state = reactive({
    themeName: '默认',
    theme: {} as Theme
  })

  const onRadioGroupChanged = (label: string) => {
    const themeValue = DEFAULT_THEMES.find(t => t.name === label)
    if (themeValue) {
      const theme = themeProcess(themeValue)
      setDocumentTheme(theme)
    }
  }
</script>
