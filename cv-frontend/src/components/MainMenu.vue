<template>
  <nav>
    <div class="menu-header-wrapper">
      <div class="profile-img-wrapper">
        <img class="profile-img" src="../assets/img/profile.jpg" alt="Michele Sessa">
      </div>
      <div class="menu-header-titles">
        <h1 class="title">Michele<br />Sessa</h1>
        <h2 class="subtitle">Software Engineer</h2>
      </div>
    </div>

    <p @click="showContactInfo = !showContactInfo" class="std-btn contact-btn">
      {{ ContactBtnText }}
    </p>

    <div v-if="showContactInfo" class="contact-info-container">
      <div class="info-section">
        <h3>Portfolio</h3>
        <div class="img-container">
          <a href="https://github.com/mikysett" target="_blank">
            <img class="portfolio-img" src="../assets/img/github_logo.svg" alt="GitHub Profile">
          </a>
          <a href="https://www.linkedin.com/in/michele-sessa/">
            <img class="portfolio-img" src="../assets/img/linkedin_logo.png" alt="LinkedIn Profile">
          </a>
        </div>
      </div>

      <div class="info-section">
        <h3>Contact info</h3>
        <p><a class="contact-link" href="mailto:mikysett@gmail.com">✉️ mikysett@gmail.com</a></p>
        <p><a class="contact-link" href="tel:+393271551904">📞 +39 327 15 51 904</a></p>
        <p>🏠 Lisbon, Portugal</p>
      </div>

      <div class="info-section">
        <h3>Languages</h3>
        <div class="skill-line">
          <div class="icon-container">🍕</div>
          <div class="skill-name">Italian</div>
          <div class="skill-level">Native</div>
        </div>
        <div class="skill-line">
          <div class="icon-container">🥖</div>
          <div class="skill-name">French</div>
          <div class="skill-level">Native</div>
        </div>
        <div class="skill-line">
          <div class="icon-container">🗽</div>
          <div class="skill-name">English</div>
          <div class="skill-level">C1</div>
        </div>
        <div class="skill-line">
          <div class="icon-container">🐓</div>
          <div class="skill-name">Portuguese</div>
          <div class="skill-level">B2</div>
        </div>
      </div>

    </div>

    <h3 class="menu-title">More about me</h3>
    <div class="bottom-menu">
      <router-link class="menu-link" to="/bio">Bio</router-link>
      <router-link class="menu-link" to="/programming">Programming</router-link>
    </div>
  </nav>
</template>

<script setup>
import { ref, computed } from 'vue'

const showContactInfo = ref(true)

if (window.innerWidth <= 850) {
  showContactInfo.value = false
}

const ContactBtnText = computed(() => {
  return showContactInfo.value ? 'Hide contact info' : 'Show contact info'
})
</script>

<style scoped>
.profile-img-wrapper {
  display: flex;
  justify-content: center;
}

.profile-img {
  border-radius: 50%;
  max-width: 180px;
}

.title {
  font-family: "Cutive Mono", monospace;
  font-weight: bold;
  font-size: 38px;
  line-height: 44px;
  margin-top: 20px;
}

.subtitle {
  font-family: "Cutive Mono", monospace;
  font-size: 18px;
}

.info-section {
  margin-top: 20px;
}

.info-section h3, .menu-title {
  font-family: "Cutive Mono", monospace;
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 8px;
}

.menu-title {
  margin-top: 20px;
}

.portfolio-img {
  max-height: 32px;
  margin-right: 12px;
}

.skill-line {
  margin-bottom: 4px;
  display: flex;
}

.skill-level {
  display: flex;
  justify-content: flex-end;
  flex: 1;
}

.bottom-menu {
  display: flex;
  flex-direction: column;
  border: solid 2px #00a851;
  padding: 4px;
}

.contact-link {
  color: var(--color1);
}

.contact-link:hover {
  color: var(--color2);
}

.menu-link {
  color: var(--color1);
  text-decoration: underline;
}

.menu-link:hover {
  color: var(--color2);
}

.contact-btn {
  display: none;
  text-align: center;
}

@media (max-width: 850px) {
  .contact-btn {
    display: block;
  }

  .menu-header-wrapper {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
  }

  .profile-img {
    max-width: 90px;
    margin-right: 20px;
  }

  .title {
    margin-top: 0;
    line-height: 38px;
  }
}

</style>
