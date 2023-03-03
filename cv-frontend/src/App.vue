<template>
  <div class="main-grid">
    <div class="side-content-wrapper">
      <main-menu />
    </div>
    <div class="main-content-wrapper">
      <router-view />
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

import MainMenu from '@/components/MainMenu'

const darkMode = ref(null)

const initStyleMode = () => {
  if (window.matchMedia &&
    window.matchMedia('(prefers-color-scheme: dark)').matches) {
    darkMode.value = true
  } else {
    darkMode.value = false
  }
  setStyleModeInDocument()
}

const setStyleModeInDocument = () => {
  if (darkMode.value === true) {
    document.documentElement.setAttribute('style-mode', 'dark')
  } else {
    document.documentElement.setAttribute('style-mode', 'light')
  }
}

// eslint-disable-next-line
const toggleStyleMode = () => {
  darkMode.value = !darkMode.value
  setStyleModeInDocument()
}

initStyleMode()
</script>

<style>
@import './assets/reset.css';
@import './assets/globals.css';

#app {
  font-family: Lato, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: var(--bg1);
}

.main-grid {
  display: grid;
  min-height: 100vh;
  grid-auto-columns: 40%;
  grid-column-gap: 0px;
  grid-row-gap: 16px;
  grid-template-columns: 30% 70%;
  grid-template-rows: auto;
}

.side-content-wrapper {
  display: flex;
  justify-content: flex-end;
  background-color: var(--bg2);
  padding: 20px;
}

.main-content-wrapper {
  padding: 20px;
}

</style>
