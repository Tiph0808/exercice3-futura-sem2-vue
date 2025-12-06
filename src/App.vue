<script setup>
import Header from './components/Header.vue'
import FrontPage from './components/FrontPage.vue'
import ArticleCard from './components/ArticleCard.vue'
import Footer from './components/Footer.vue'
import data from './assets/articles.json'
console.log(data)

const articleArray = data.articlesList
</script>

<template>
  <Header />
  <main class="wrapper">
    <FrontPage :infos="data.frontPage" />

    <ArticleCard :articleArray="articleArray" />
  </main>
  <Footer />
</template>

<style scoped></style>
