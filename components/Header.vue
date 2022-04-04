<template>
  <el-menu mode="horizontal" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
    <el-menu-item index="1"
      > <NuxtLink to="/">首页</NuxtLink></el-menu-item
    >
    <el-menu-item index="2"
      ><router-link to="/">健康</router-link></el-menu-item
    >

    <el-menu-item index="3" disabled>时尚</el-menu-item>
    <el-menu-item index="4">游戏</el-menu-item>
    <el-menu-item index="5">数码</el-menu-item>
    <el-menu-item index="6">金融</el-menu-item>
    <el-menu-item index="7">
      <NuxtLink to="/articles">文章</NuxtLink>
      </el-menu-item>
  </el-menu>
</template>
