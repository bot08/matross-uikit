<template>
    <div @click="themeSwitch()" class="dark:bg-gray-800 bg-gray-200
                                         relative flex-shrink-0 cursor-pointer
                                         h-[34px] w-[66px] 
                                         border-2 border-transparent 
                                         rounded-full 
                                         transition-colors ease-in-out focus:outline-none">
        <span class="sr-only">Theme switch</span>
        <span class="dark:translate-x-8 translate-x-0 
                     pointer-events-none inline-block ring-0
                     h-[30px] w-[30px] 
                     rounded-full bg-white dark:bg-gray-200 shadow-lg 
                     transform transition ease-in-out"/>
    </div>
</template>


<script setup>
function themeSwitch() {
    const html = document.querySelector("html");
    if(localStorage.getItem('theme')=="dark"){
        html.classList.remove("dark");
        localStorage.setItem("theme", "white");
        document.querySelector('meta[name="theme-color"]').setAttribute("content", "#f9fafb");
    }
    else{
        html.classList.add("dark");
        localStorage.setItem("theme", "dark");
        document.querySelector('meta[name="theme-color"]').setAttribute("content", "#374151");
    }
}
</script>
