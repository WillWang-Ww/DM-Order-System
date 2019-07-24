<template>
<el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
  <el-menu-item index="1">主页</el-menu-item>
  <el-menu-item index="1">菜单</el-menu-item>
  <el-menu-item index="1">管理</el-menu-item>
  <el-menu-item index="1">关于我们</el-menu-item>
</el-menu>
</template>

<script>
   export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>
