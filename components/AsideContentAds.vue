<script>
export default {};
</script>

<template>
  <el-card shadow="always">
    <div v-for="o in 4" :key="o" class="text item">
      {{ "List item " + o }}
    </div>
  </el-card>

</template>