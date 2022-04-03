<template>
  <div>
    <ul v-if="articles.length">
      <li v-for="article of articles" :key="article.slug">
        <NuxtLink :to="'/articles/'+ article.slug">{{
          article.slug
        }}</NuxtLink>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  
  async asyncData({$content}) {
    const articles = await $content("notes")
      .sortBy("createdAt", "asc")
    //   .limit(12)
      .fetch();
    return {articles}
  },
};
</script>