<script setup>

const message = ref('Nuxt')
const appConfig = useAppConfig()
function hello () {
  sayHello(message.value)
}
</script>

<template className="dark">
  <v-app>
    <NavBar/>
    <NuxtPage/>
  </v-app>
</template>

<style>
@import './assets/styles/main.css';
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
</style>

