<template>
  <section class="articleContent">
    <p class="userName">{{ author }}</p>
    <h2 class="articleName">{{ title }}</h2>
    <p class="createDate">{{ date }}</p>
    <section class="textContent">
      <h3 class="contentTitle">{{ summary }}</h3>
      <p>{{ content }}</p>
    </section>
  </section>
</template>

<script>
export default {
  name: "Article",
  props: {
    author: String,
    title: String,
    date: String,
    summary: String,
    content: String,
  },
};
</script>

<style>
/* ここにスタイルを追加してください */
</style>
