<template>
  <el-container>
    <el-header><Header></Header></el-header>
    <el-main>
      <el-row :gutter="10">
        <el-col :md="18"><Nuxt/></el-col>
        <el-col :md="6" class="hidden-sm-and-down">
          <AsideContentAds></AsideContentAds>
          <!-- <el-backtop target=".page-component__scroll .el-scrollbar__wrap" :bottom="40">up</el-backtop> -->
        </el-col>
      </el-row>
    </el-main>
  </el-container>
</template>

<script>
</script>

<style>
.el-container {
  background-color: #e9e9eb;
}
</style>