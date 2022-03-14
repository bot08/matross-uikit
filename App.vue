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
    
  </main>
</template>


<script setup>
import ThemeToggle from './components/ThemeToggle.vue'
import Button from './components/Button.vue'
import ButtonLoading from './components/ButtonLoading.vue'
</script>