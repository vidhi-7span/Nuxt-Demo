<template class="flex">
  <nav
    class="flex justify-between items-center px-6 py-4 bg-slate-400 shadow-lg"
  >
    <img
      src="https://pbs.twimg.com/media/GCsrWLFXsAAgEVa?format=png&name=large"
      alt=""
      class="h-19 w-24 rounded-full"
    />
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
