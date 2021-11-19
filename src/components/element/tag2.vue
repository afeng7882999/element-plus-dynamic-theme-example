<template>
  <el-tag v-for="tag in tags" :key="tag.name" closable :type="tag.type">
    {{ tag.name }}
  </el-tag>
  <div class="tag-group">
    <span class="tag-group__title">Dark</span>
    <el-tag
        v-for="item in items"
        :key="item.label"
        :type="item.type"
        effect="dark"
    >
      {{ item.label }}
    </el-tag>
  </div>
  <div class="tag-group">
    <span class="tag-group__title">Plain</span>
    <el-tag
        v-for="item in items"
        :key="item.label"
        :type="item.type"
        effect="plain"
    >
      {{ item.label }}
    </el-tag>
  </div>
  <div>
    <el-check-tag checked style="margin-right: 8px">Checked</el-check-tag>
    <el-check-tag :checked="checked" @change="onChange">Toggle me</el-check-tag>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      tags: [
        { name: 'Tag 1', type: '' },
        { name: 'Tag 2', type: 'success' },
        { name: 'Tag 3', type: 'info' },
        { name: 'Tag 4', type: 'warning' },
        { name: 'Tag 5', type: 'danger' },
      ],
      items: [
        { type: '', label: 'Tag 1' },
        { type: 'success', label: 'Tag 2' },
        { type: 'info', label: 'Tag 3' },
        { type: 'danger', label: 'Tag 4' },
        { type: 'warning', label: 'Tag 5' },
      ],
      checked: false,
    }
  },
  methods: {
    onChange(checked) {
      this.checked = checked
    },
  },
}
</script>
