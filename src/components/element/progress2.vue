<template>
  <div class="demo-progress">
    <el-progress :percentage="50">
      <el-button type="text">Content</el-button>
    </el-progress>
    <el-progress
        :text-inside="true"
        :stroke-width="20"
        :percentage="50"
        status="exception"
    >
      <span>Content</span>
    </el-progress>
    <el-progress type="circle" :percentage="100" status="success">
      <el-button type="success" :icon="Check" circle></el-button>
    </el-progress>
    <el-progress type="dashboard" :percentage="80">
      <template #default="{ percentage }">
        <span class="percentage-value">{{ percentage }}%</span>
        <span class="percentage-label">Progressing</span>
      </template>
    </el-progress>
  </div>
  <div class="demo-progress">
    <el-progress :percentage="50" :indeterminate="true" />
    <el-progress :percentage="100" :format="format" :indeterminate="true" />
    <el-progress
        :percentage="100"
        status="success"
        :indeterminate="true"
        :duration="5"
    />
    <el-progress
        :percentage="100"
        status="warning"
        :indeterminate="true"
        :duration="1"
    />
    <el-progress :percentage="50" status="exception" :indeterminate="true" />
  </div>
</template>

<script setup lang="ts">
import { Check } from '@element-plus/icons'

const format = (percentage: any) => percentage === 100 ? 'Full' : `${percentage}%`
</script>

<style lang="scss" scoped>
.percentage-value {
  display: block;
  margin-top: 10px;
  font-size: 28px;
}

.percentage-label {
  display: block;
  margin-top: 10px;
  font-size: 12px;
}
</style>
