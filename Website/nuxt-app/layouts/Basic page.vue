<template>
  <div class="flex flex-col min-h-screen">
    <nav class="bg-blue-600 text-white p-4">
      <div class="container mx-auto flex justify-between">
        <h1 class="text-lg font-bold">My Website</h1>
        <ul class="flex space-x-4">
          <li><NuxtLink to="/" class="hover:underline">Home</NuxtLink></li>
          <li><NuxtLink to="/about" class="hover:underline">About</NuxtLink></li>
        </ul>
      </div>
    </nav>

    <main class="flex-1 container mx-auto p-5">
      <slot />
    </main>

    <footer class="bg-gray-800 text-white text-center p-3">
      © 2025 HELFY
    </footer>
  </div>
</template>