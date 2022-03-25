<template>
  <main>
    <!-- Theme toggle -->
    <div class="bg-gray-50 dark:bg-gray-700 transition-colors w-full p-4 mb-2">
      <ThemeToggle/>
    </div>

    <!-- Button on background -->
    <div class="bg-gray-50 dark:bg-gray-700 transition-colors w-full p-4 my-2">
      <Button/>
    </div>
    <!-- Without background -->
    <Button class="m-4"/>

    <!-- Loading button on background -->
    <div class="bg-gray-50 dark:bg-gray-700 transition-colors w-full p-4 my-2">
      <ButtonLoading/>
    </div>
    <!-- Without background -->
    <ButtonLoading class="m-4"/>

    <!-- Items -->
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5">
      <ItemCard/>
      <ItemCard/>
      <ItemCard/>
      <ItemCard/>
      <ItemCard/>
      <ItemCard/>
      <ItemCard/>
      <ItemCardPreloader/>
      <ItemCardPreloader/>
      <ItemCardPreloader/>
    </div>

    <!-- Container (example) -->
    <div class="mx-auto max-w-7xl 
                 px-4 sm:px-6 lg:px-8 
                 pt-18 sm:pt-20 lg:pt-24 xl:pt-26">
    </div>

    <!-- Big text -->
    <h3 class="text-3xl font-extrabold leading-9 tracking-tight sm:leading-10">
      Text example
    </h3>
    <!-- Medium text -->
    <h4 class="font-bold text-xl">
      Text example
    </h4>
    <!-- Small text -->
    <p class="text-lg text-gray-900 dark:text-gray-200">
      Text example
    </p>
  </main>
</template>


<script setup>
import ThemeToggle from './components/ThemeToggle.vue'
import Button from './components/Button.vue'
import ButtonLoading from './components/ButtonLoading.vue'
import ItemCard from './components/ItemCard.vue'
import ItemCardPreloader from './components/ItemCardPreloader.vue'
</script>