<script setup>
const props = defineProps({
  infos: Object,
})

console.log(props.infos)
</script>

<template>
  <div :style="{ backgroundImage: `url(${infos.image})` }" class="container">
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
.container {
  height: 550px;
  background-repeat: no-repeat;
  background-size: 100%;
  padding: 80px;
}
</style>
