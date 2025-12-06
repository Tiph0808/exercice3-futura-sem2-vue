<script setup>
const props = defineProps({
  infos: Object,
})
</script>

<template>
  <div
    class="front-page"
    :style="{ backgroundImage: `url(${infos.image})`, backgroundSize: `contain` }"
  >
    <div>
      <h3>
        <span>{{ infos.category }}</span
        ><span>{{ infos.subCategory }}</span>
      </h3>
      <h1>{{ infos.title }}</h1>
    </div>
    <p>{{ infos.teaser }}</p>
  </div>
</template>

<style scoped>
.front-page {
  height: 550px;
  border: 1px solid blue;
  padding: 80px;
}
</style>
