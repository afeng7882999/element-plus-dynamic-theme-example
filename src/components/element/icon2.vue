<template>
  <div style="font-size: 20px;">
    <!-- Since svg icons do not carry any attributes by default -->
    <!-- You need to provide attributes directly -->
    <edit style="width: 1em; height: 1em; margin-right: 8px;"/>
    <share style="width: 1em; height: 1em; margin-right: 8px;"/>
    <delete style="width: 1em; height: 1em; margin-right: 8px;"/>
    <search style="width: 1em; height: 1em; margin-right: 8px;"/>
  </div>
  <el-icon :size="20">
    <edit/>
  </el-icon>
  <el-icon color="#409EFC" class="no-inherit">
    <share/>
  </el-icon>
  <el-icon>
    <delete/>
  </el-icon>
  <el-icon class="is-loading">
    <loading/>
  </el-icon>
  <el-button type="primary">
    <el-icon style="vertical-align: middle;">
      <search/>
    </el-icon>
    <span style="vertical-align: middle;"> Search </span>
  </el-button>
</template>

<script setup lang="ts">
import { Edit, Share, Delete, Search, Loading } from "@element-plus/icons";
</script>
