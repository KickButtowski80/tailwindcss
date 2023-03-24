<template lang="">
  <div class="">
    <div class="px-8 py-12 max-w-md sm:max-w-2xl
                mx-auto lg:px-10 lg:py-24
                lg:max-w-full xl:mr-0 2xl:mx-auto
                2xl:col-span-2">

      <h1 class="text-xl text-gray-900">Popular Destinations</h1>
      <p class='mt-2 text-gray-600 '>A selection of great vue 3 friendly citites with lots to
        see and explore
      </p>    
      <div class="mt-6 grid gap-3 md:gap-6 md:grid-cols-2 2xl:grid-cols-3">
        <div v-for="{city,imageUrl,averagePrice,propertyCount,imageAlt} of popularDestinations"
              :key='city'>
        <div class="flex items-center rounded-lg
                  bg-white shadow-lg overflow-hidden">               
            <img :src="imageUrl" :alt="imageAlt"
            class="h-40 w-32 md:h-64 md:w-40
                  max-w-md object-cover object-center
                  flex-shrink-0 rounded-lg">
            <div class="px-6 py-4 flex-shrink-1">
              <div class="text-sm md:text-lg lg:text-2xl
                          font-semibold text-gray-800">
                <h3>{{city}}</h3>
                <p class="text-gray-600">${{averagePrice}}/night average</p>
                <div class="mt-2">
                  <a href="#" class="text-green-500 hover:text-green-400 font-semibold text-sm">
                    Explore {{propertyCount }} properties
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>  
  </div>
</template>
<script>
import popularDestinations from '../data/popularDestinations';
export default {
  data() {
    return {
      popularDestinations: popularDestinations
    }
  }

}
</script>
<style lang="">
  
</style>
