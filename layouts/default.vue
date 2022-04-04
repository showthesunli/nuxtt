<template>
  <el-row>
    <el-col>
      <el-container>
        <el-header><Header></Header></el-header>
        <el-main>
          <el-row :gutter="10">
            <el-col :md="18"><Nuxt></Nuxt></el-col>
            <el-col :md="6" class="hidden-sm-and-down">
              <AsideContentAds></AsideContentAds>
              <!-- <el-backtop target=".page-component__scroll .el-scrollbar__wrap" :bottom="40">up</el-backtop> -->
            </el-col>
          </el-row>
        </el-main>
        <el-backtop target=".el-container " :bottom="100">
          <div
            style="
               {
                height: 100%;
                width: 100%;
                background-color: #f2f5f6;
                box-shadow: 0 0 6px rgba(0, 0, 0, 0.12);
                text-align: center;
                line-height: 40px;
                color: #1989fa;
              }
            "
          >
            UP
          </div>
        </el-backtop>
      </el-container>
    </el-col>
  </el-row>
</template>

<script>
</script>

<style>
.el-row {
  background-color: #e9e9eb;
}
</style>