<template >
  <div class="">
    <div class="
      px-8 py-12 max-w-md
      sm:max-w-2xl mx-auto
      lg:px-10 lg:py-24 lg:max-w-full
      xl:mr-0 2xl:mx-auto 2xl:col-span-2">
      <h1 class="text-3xl text-gray-900 font-semibold">Popular Destinations</h1>
      <p class="md:text-2xl mt-2 text-gray-600
                md:font-semibold">
        A selection of great vue 3 friendly citites with lots to see and explore
      </p>
      <div class="mt-6 grid gap-3 md:gap-6
                 sm:grid-cols-2 2xl:grid-cols-3">
        <div v-for="{
          city,
          imageUrl,
          averagePrice,
          propertyCount,
          imageAlt,
        } of popularDestinations" :key="city" class="relative">
          <img :src="imageUrl" :alt="imageAlt" class=" 
              
               w-full md:h-64
               object-cover object-center
               rounded-lg" />
          <div class="text-lg md:text-sm
              font-bold lg:text-2xl">
            <div class="bg-white bg-opacity-70 hover:bg-opacity-90
                       backdrop-filter  backdrop-blur-xs
                       absolute top-0 left-0 translate-x-full                    
                       w-1/2 h-full text-center
                       flex flex-col justify-center text-gray-500 
                       hover:text-green-700  rounded-lg  ">
              <h3 class="text-lg md:text-2xl">{{ city }}</h3>
              <p class="text-sm md:text-base">${{ averagePrice }}/night average</p>
              <div class="mt-2">
                <a href="#" class="text-white-500 
                   font-semibold text-sm">
                  Explore {{ propertyCount }} properties
                </a>
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
      popularDestinations: popularDestinations,
    };
  },
};
</script>
<style lang=""></style>
