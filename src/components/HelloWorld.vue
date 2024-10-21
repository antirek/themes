<script setup>

// import '../themes/default/HelloWorld.css'
const theme = import.meta.env.THEME;
console.log('theme', theme);
// const path = `../themes/${theme}/HelloWorld.css`

// if (theme === 'light-green') {
import '../themes/green-light/HelloWorld.css'
// } else {
// import '../themes/default/HelloWorld.css'
// }



defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      <a href="https://vite.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
  </div>
</template>
