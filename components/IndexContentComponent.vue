<template>
  <el-row :gutter="20" >
    <el-col :key="n" v-for="n in 20" :xs="24" :sm="12" :md="8">
      <el-card shadow="hover" style="margin-bottom: 20px">
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

</script>