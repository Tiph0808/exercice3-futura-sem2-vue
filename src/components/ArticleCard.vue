<script setup>
const props = defineProps({
  articleArray: Array,
})

console.log(props)
</script>

<template>
  <section class="articles">
    <div v-for="article in articleArray" :key="article.id">
      <img :src="article.image" alt="" />
      <h3>
        <span>{{ article.category }}</span>
        <span>{{ article.subCategory }}</span>
      </h3>
      <p>{{ article.title }}</p>
      <p>{{ article.date }}</p>
    </div>
  </section>
</template>

<style scoped>
.articles {
  border: 2px solid palevioletred;
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  padding: 50px 20px 30px 20px;
}

.articles > div {
  border: 2px solid green;
  height: 480px;
  width: 290px;
}

img {
  height: 70%;
  width: 100%;
  object-fit: cover;
}
</style>
