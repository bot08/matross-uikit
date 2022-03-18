<template>
    <div class="rounded-lg mt-1 mb-4 md:mb-8 overflow-hidden shadow-lg bg-gray-50 dark:bg-gray-700 text-gray-900 dark:text-gray-100 transition-colors sm:mx-auto sm:text-center sm:w-48">
        <a class="flex sm:block">
            <HomeIcon class="w-20 h-20 sm:w-28 sm:h-28 sm:m-auto rounded-xl mx-3 my-3 sm:mb-0 drop-shadow"/>
            <div class="px-3 py-1 my-auto">
                <h1 class="font-bold mb-1 sm:mt-1 sm:mb-2 text-xl">Главная</h1>
            </div>
        </a>
    </div>
</template>


<script setup>
import { HomeIcon } from '@heroicons/vue/solid'
</script>
