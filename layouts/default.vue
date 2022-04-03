<template>
  <el-row>
    <el-col :span="18" :offset="3">
      <el-container>
        <el-header><Header></Header></el-header>

        <el-main><Nuxt></Nuxt></el-main>
      </el-container>
    </el-col>
  </el-row>
</template>

<script>

</script>

<style>
.el-row {
  background-color: #e9e9eb
}

</style>