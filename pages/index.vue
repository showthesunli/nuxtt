<template>
  <index-content-component></index-content-component>
</template>


<script>
export default {
  async asyncData({$content}){
    const articleListAtIndex = $content("notes")
  }
};
</script>