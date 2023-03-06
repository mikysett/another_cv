<template>
  <div class="header-container">
    <h1>{{ props.pageName }}</h1>
    <div class="header-btn-container">
      <router-link to="/">Back to Home</router-link>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(['pageName'])
</script>

<style scoped>
</style>
