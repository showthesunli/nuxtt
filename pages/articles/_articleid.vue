<template>
  <article>
    <nuxt-content :document="article" />
    <el-row>
      <el-col :span="12">
        <el-link type="primary" v-if="prev" @click="$router.push({name:'articles-articleid', params:{articleid:prev.slug}})">上一章：{{ prev.slug }}</el-link>
      </el-col>
      <el-col :span="12">
        <el-link type="primary" v-if="next" @click="$router.push({name:'articles-articleid',params:{articleid:next.slug}})">下一章：{{next.slug}}</el-link>
      </el-col>
    </el-row>
  </article>
</template>
<script>
export default {
  
  async asyncData({ $content, params }) {
    const article = await $content("notes", params.articleid).fetch();
    const [prev, next] = await $content("notes")
      .only(["path", "slug"])
      .sortBy("date")
      .surround(params.articleid)
      .fetch();

    return {
      article,
      prev,
      next,
    };
  },
};
</script>