<template>
  <div class="bg-gray-100 h-full">
    <header class="bg-white shadow h-16 flex justify-between items-stretch">
      <router-link
        :to="{ name: 'home' }"
        class="inline-flex items-center h-full px-5"
      >
        Home
      </router-link>
      <div class="flex items-center gap-1">
        <router-link
          :to="{ name: 'byName' }"
          class="flex items-center px-2 h-full transition-all hover:bg-purple-100"
        >
          Search Meals
        </router-link>
        <router-link
          :to="{ name: 'byLetter' }"
          class="flex items-center px-2 h-full transition-all hover:bg-purple-100"
        >
          Meals By Letter
        </router-link>
        <router-link
          :to="{ name: 'byIngredient' }"
          class="flex items-center px-2 h-full transition-all hover:bg-purple-100"
        >
          Meals By Ingredients
        </router-link>
      </div>
    </header>
    <main>
      <router-view></router-view>
    </main>
  </div>
</template>

<script setup></script>

<style scoped></style>
