<script setup>
// import { RouterLink, RouterView } from "vue-router";
// import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <header>自动化测试报告模板</header>
  <div class="template-wrapper">
    <router-view></router-view>
  </div>
</template>

<style>
@import "@/assets/base.css";

header {
  height: 54px;
  padding: 10px;
  line-height: 2.2rem;
}

.template-wrapper {
  display: grid;
  grid-template-columns: 400px auto;
  height: 100%;
  height: calc(100vh - 54px);
  overflow: auto;
}
</style>
