<template>
  <div class="wrapper">
    <PageHeader />
    <NavigationMenu />
    <main class="mainContent">
      <ArticleContent
        :author="author"
        :title="title"
        :date="date"
        :summary="summary"
        :content="content"
      />
    </main>
    <PageFooter />
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import NavigationMenu from "./components/NavigationMenu.vue";
import ArticleContent from "./components/ArticleContent.vue";
import PageFooter from "./components/PageFooter.vue";

export default {
  name: "App",
  components: {
    PageHeader,
    NavigationMenu,
    ArticleContent,
    PageFooter,
  },
  data() {
    return {
      author: "Qiita User",
      title: "記事タイトル",
      date: "2022/01/01",
      summary: "記事の概要",
      content: "記事の本文",
    };
  },
};
</script>

<style>
/* Add your styles here */
</style>
