<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="px-8 py-12">
    <div class="m-8 flex">
      <img src="./assets/vue.svg" class="w-10 h-10 mr-6" alt="Vue logo" />
      <h3 class="text-3xl font-bold">Working Vue 3</h3>
    </div>
    <img src="https://nypost.com/wp-content/uploads/sites/2/2023/01/shutterstock_1770576515.jpg?quality=75&strip=all"
      alt="" class="h-auto max-w-md
                        rounded-lg shadow-2xl">
    <h1 class="mt-6 text-2xl font-bold text-gray-700">You can Vue 3 from anywhere.
      <br>
      <span class="text-green-500 ">Take advantage of it.</span>
    </h1>
    <p class="mt-2 text-gray-600 max-w-md ">
      Vue3 helps you to desing interactive web pages.
      It is easy to learn and easy to start.
      Let's make world an easier world by using Vue 3.
      Vue forever
    </p>
    <div class="mt-8">
      <a href="#" class=" inline-block px-5 py-3 rounded-lg
              bg-green-500
              text-gray-500 shadow-xl
              upercase tracking-wider
              font-semibold text-sm">Let's Vue Today</a>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
