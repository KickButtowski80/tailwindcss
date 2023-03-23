<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="grid  lg:grid-cols-2 2xl:grid-cols-5
                    bg-gray-100">
    <div class="px-8 py-12 max-w-md sm:max-w-xl mx-auto lg:px-10 lg:py-24
                    lg:max-w-full xl:mr-0 2xl:mx-auto 2xl:col-span-2">
      <div class="xl:max-w-xl">
        <div class="flex items-center">
          <img src="./assets/vue.svg" class="w-10 h-10
                     md:w-16 mb-3" alt="Vue logo" />
          <h3 class="text-base md:text-3xl font-bold pl-3">Working Vue 3</h3>
        </div>
        <img src="https://nypost.com/wp-content/uploads/sites/2/2023/01/shutterstock_1770576515.jpg?quality=75&strip=all"
          alt="" class="rounded-lg shadow-2xl
                              mt-4 sm:h-64 sm:w-full
                              sm:object-cover sm:object-top
                              lg:hidden">
        <h1 class="mt-6 text-base
                        font-bold text-gray-700
                        sm:mt-8 sm:text-3xl lg:text-2xl xl:text-4xl">You can Vue 3 from anywhere.
          <br class="">
          <span class="text-green-500 ">Take advantage of it.</span>
        </h1>
        <p class="mt-2 sm:text-xl sm:mt-3 text-gray-600">
          Vue3 helps you to desing interactive web pages.
          It is easy to learn and easy to start.
          Let's make world an easier world by using Vue 3.
          View Life with Vue 3 forever 💌
        </p>
        <div class="mt-4 sm:mt-6">
          <a href="#" class=" inline-block px-5 py-3 rounded-lg
                        bg-green-500
                        text-gray-500 shadow-xl
                        uppercase tracking-wider
                        font-semibold text-sm sm:text-base">Let's Vue Today</a>
        </div>
      </div>
    </div>
    <div class="hidden relative lg:block 2xl:col-span-3 ">
      <img src="https://nypost.com/wp-content/uploads/sites/2/2023/01/shutterstock_1770576515.jpg?quality=75&strip=all"
        alt="" class="absolute inset-0 w-full h-full object-cover object-center">
    </div>
  </div>
</template>


