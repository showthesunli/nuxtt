<template>
  <div>
    <NuxtLink to="/articles">文章列表</NuxtLink>
    <Nuxt-Link to="/articles/hello">hello.md</Nuxt-Link>
    <Nuxt-Link to="/articles/hi">hi.md</Nuxt-Link>

    <article>
      <nuxt-content :document="page" />
    </article>
  </div>
</template>


<script>
export default {
  async asyncData({ $content, route }) {
    const page = await $content("hello").fetch();

    return {
      page,
    };
  },
};
</script>