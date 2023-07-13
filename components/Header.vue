<template>
  <header class="bg-transparent text-gray-900 py-4 px-64">
    <nav class="flex justify-between items-center">
      <div class="flex items-center">
        <img class="mr-8 h-10" src="/assets/logo1.png" alt="Logo" />
        <h1 class="text-2xl font-black">
          <router-link to="/" :class="{ 'text-black': $route.path === '/' }">
            joshualeegarza
          </router-link>
        </h1>
      </div>
      <div class="flex items-center">
        <router-link
          to="/"
          class="text-black font-semibold hover:text-teal-700 mx-3"
          :class="{ 'text-black': $route.path === '/' }"
        >
          Home
        </router-link>
        <router-link
          to="/about"
          class="text-black font-semibold hover:text-teal-700 mx-3"
          :class="{ 'text-black': $route.path === '/about' }"
        >
          About
        </router-link>
        <router-link
          to="/projects"
          class="text-black font-semibold hover:text-teal-700 mx-3"
          :class="{ 'text-black': $route.path === '/projects' }"
        >
          Projects
        </router-link>
        <router-link
          to="/blog"
          class="text-black font-semibold hover:text-teal-700 mx-3"
          :class="{ 'text-black': $route.path === '/blog' }"
        >
          Blog
        </router-link>
        <router-link
          to="/contact"
          class="text-black font-semibold hover:text-teal-700 mx-3"
          :class="{ 'text-black': $route.path === '/contact' }"
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
