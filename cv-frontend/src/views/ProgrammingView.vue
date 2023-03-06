<template>
  <div class="main-container">
    <div class="header-container">
      <h1>Programming</h1>
      <div class="header-btn-container">
        <router-link to="/">Back to Home</router-link>
      </div>
    </div>
    <Separator />
  </div>
</template>

<script>
import Separator from '@/components/Separator.vue'

export default {
  name: 'ProgrammingView',
  components: {
    Separator
  }
}
</script>

<style scoped>
</style>
