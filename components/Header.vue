<template>
  <header class="bg-gray-900 text-white py-4 px-6">
    <nav class="flex justify-between items-center">
      <div class="flex items-center">
        <h1 class="text-2xl font-bold">My Website</h1>
      </div>
      <div class="flex items-center">
        <router-link
          to="/"
          class="mr-4 py-2 px-3 rounded-lg hover:bg-gray-800"
          :class="{ 'bg-gray-800': $route.path === '/' }"
        >
          Home
        </router-link>
        <router-link
          to="/about"
          class="mr-4 py-2 px-3 rounded-lg hover:bg-gray-800"
          :class="{ 'bg-gray-800': $route.path === '/about' }"
        >
          About
        </router-link>
        <router-link
          to="/contact"
          class="py-2 px-3 rounded-lg hover:bg-gray-800"
          :class="{ 'bg-gray-800': $route.path === '/contact' }"
        >
          Contact
        </router-link>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
/* Add custom styles here */
</style>
