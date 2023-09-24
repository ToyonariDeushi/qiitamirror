<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import Header from "./components/Header.vue";
import Navigation from "./components/Navigation.vue";
import Article from "./components/Article.vue";
import SiteFooter from "./components/SiteFooter.vue";
import SiteFooter from "./components/SiteFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Navigation,
    Article,
  },
  data() {
    return {
      author: "名前",
      title: "ちょっとした気配りで皆を幸せにする GitHub の使い方",
      date: "投稿日 2023年09月18日",
      summary: "TL;DR",
      content: "本文",
    };
  },
};
</script>

<template>
  <div class="wrapper">
    <Header />
    <Navigation />
    <main class="mainContent">
      <Article
        :author="author"
        :title="title"
        :date="date"
        :summary="summary"
        :content="content"
      />
    </main>
  </div>
</template>

<style></style>
