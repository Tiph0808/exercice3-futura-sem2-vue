<script setup></script>

<template>
  <div class="header">
    <h1>FUTURA</h1>
    <div class="fields">
      <select>
        <option>SCIENCES</option>
      </select>
      <select>
        <option>SANTE</option>
      </select>
      <select>
        <option>TECH</option>
      </select>
      <select>
        <option>MAISON</option>
      </select>
      <select>
        <option>PLANET</option>
      </select>
    </div>
    <button>JE M'ABONNE</button>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background: linear-gradient(to right, #be80ff, #6325ff);
}

.fields {
  display: flex;
  gap: 10px;
}
</style>
