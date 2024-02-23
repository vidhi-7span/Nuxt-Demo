<template class="flex">
  <nav
    class="flex justify-between items-center px-6 py-4 bg-slate-400 shadow-lg"
  >
    <h1 class="text-2xl font-bold">Demo</h1>
    <ul class="flex gap-3">
      <li><NuxtLink to="/">Home</NuxtLink></li>
      <li><NuxtLink to="/about">About Us</NuxtLink></li>
      <li><NuxtLink to="/contact">Contact</NuxtLink></li>
    </ul>
  </nav>
</template>
<style>
.router-link-active {
  @apply bg-gray-800 py-2 px-4 text-white rounded-full font-bold;
}
</style>
