<script>
export default {};
</script>

<template>
  <div>
    <el-card shadow="always" style="margin-bottom: 20px">
      <div v-for="o in 4" :key="o" class="text item">
        {{ "List item " + o }}
      </div>
    </el-card>

    <el-card shadow="always">
      <div v-for="o in 4" :key="o" class="text item">
        {{ "List item " + o }}
      </div>
    </el-card>
  </div>
</template>