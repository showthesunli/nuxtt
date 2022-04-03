<template>
  <el-row :gutter="20" style="margin-bottom: 20px">
    <el-col :key="n" v-for="n in 20" :span="8">
      <el-card shadow="hover">
        <template #header>
          <div class="card-header">
            <span>Card name</span>
            <el-button class="button" type="text">Operation button</el-button>
          </div>
        </template>
        <div v-for="o in 4" :key="o" class="text item">
          {{ "List item " + o }}
        </div>
      </el-card>
    </el-col>
  </el-row>
</template>

<script>
import AsideContentAds from "./AsideContentAds.vue";
export default {
  components: {
    AsideContentAds,
  },
};
</script>