<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class=" text-slate-900 sticky top-6 z-10">
    <div
      class="flex justify-between items-center text-gray-700 px-4 py-3 max-w-[90%] mx-auto shadow-md bg-white bg-opacity-80 rounded-full">
      <nav class="flex items-center space-x-4 px-4">
        <RouterLink class="" to="/">
          <img class=" w-20" src="https://nagad.com.bd/_nuxt/img/new-logo.7939432.png" alt="logo">
        </RouterLink>
        <RouterLink class="hover:border-b-2 hover:text-blue-600 border-blue-600" to="/">Home</RouterLink>
        <RouterLink class="hover:border-b-2 hover:text-blue-600 border-blue-600" to="/about">About</RouterLink>
        <RouterLink class="hover:border-b-2 hover:text-blue-600 border-blue-600" to="/about">Services</RouterLink>
        <RouterLink class="hover:border-b-2 hover:text-blue-600 border-blue-600" to="/about">Team</RouterLink>
        <RouterLink class="hover:border-b-2 hover:text-blue-600 border-blue-600" to="/about">Contact</RouterLink>
      </nav>
      <div class="">
        <div class="flex flex-row items-center right-1">
          <button
            class="p-2 flex flex-row items-center border border-gray-300 text-sm font-medium text-gray-700 hover:bg-gray-100 focus:bg-gray-200 focus:outline-none">
            <span class="text-md">En</span>
            <span class="ml-1">
              <img src="https://img.icons8.com/?size=512&id=t3NE3BsOAQwq&format=png" class="w-5 h-5" /></span>
          </button>

          <button
            class="p-2 flex flex-row items-center border border-gray-300 text-sm font-medium text-gray-700 hover:bg-gray-100 focus:bg-gray-200 focus:outline-none">
            <span class="text-md">Tr</span>
            <span class="ml-1">
              <img src="https://img.icons8.com/?size=512&id=7PhX5XSLeDb9&format=png" class="w-5 h-5" /></span>
          </button>
        </div>
      </div>
    </div>
  </header>
  <RouterView />
</template>

<style scoped></style>
