<template>
  <div class="justified-header header-container">
    <div class="jh-left">
      <h1>{{ props.pageName }}</h1>
    </div>
    <div class="jh-right header-btn-container">
      <router-link class="std-btn" to="/">Back&nbsp;to&nbsp;Home</router-link>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(['pageName'])
</script>

<style scoped>
h1 {
  font-family: "Cutive Mono", monospace;
  font-size: 42px;
  line-height: 1.2;
  color: var(--color2);
  font-weight: bold;
  margin-right: 20px;
}

@media (max-width: 850px) {
  .justified-header {
    flex-wrap: wrap;
  }
}
</style>
