<template>
  <div class="main-container">
    <MainHeader page-name="Programming" />

    <blockquote>
      “What I hear, I forget; What I see, I remember; What I do, I understand.”
      <br>
      <strong>― Confucius, 551-479 BC</strong>
    </blockquote>

    <Separator />

  </div>
</template>

<script>
import Separator from '@/components/Separator.vue'
import MainHeader from '@/components/MainHeader.vue'

export default {
  name: 'ProgrammingView',
  components: {
    Separator,
    MainHeader
  }
}
</script>

<style scoped>
</style>
