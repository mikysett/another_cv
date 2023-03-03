<template>
  <div class="main-container">
    <blockquote>
      “Programs must be written for people to read, and only incidentally for machines to&nbsp;execute.”
      <br>
      <strong>― Abelson & Sussman</strong>
    </blockquote>

    <Separator />

    <div class="job-container">
      <div class="company-container">
        <div class="justified-header">
          <div class="jh-left">
            <h2>01 Talent</h2>
          </div>
          <div class="jh-right">
            <p>Lisbon, Portugal</p>
          </div>
        </div>
        <div class="description">
          01Talent provide peer2peer learning platforms and pedagogical content to train high-level programmers worldwide.
        </div>
      </div>

      <div class="roles-wrapper">
        <div class="role-wrapper">
          <h3 class="role-title">Junior Software Engineer</h3>
          <div class="justified-header">
            <div class="jh-left">
              <p>Full-time</p>
            </div>
            <div class="jh-right">
              <p>Jan 2023 - Present</p>
            </div>
          </div>
          <div class="description">
            Improve the pedagogical team infrastructure creating standardized workflows and automations to streamline
            content creation and minimize friction points in production cycles.
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import Separator from '@/components/Separator.vue'

export default {
  name: 'HomeView',
  components: {
    Separator
  }
}
</script>

<style scoped>
</style>
