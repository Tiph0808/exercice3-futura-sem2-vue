<script setup>
const props = defineProps({
  articleInfos: Object,
})
</script>

<template>
  <div>
    <img :src="articleInfos.image" alt="" />
    <p>
      <span>{{ articleInfos.category }}</span
      ><span>{{ articleInfos.subCategory }}</span>
    </p>

    <h2>{{ articleInfos.title }}</h2>

    <p>{{ articleInfos.date }}</p>
  </div>
</template>

<style scoped>
img {
  height: 100px;
  width: 100px;
}
</style>
