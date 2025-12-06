<template>
  <div class="min-h-screen bg-slate-50 text-slate-900 font-sans">
    <Navbar />
    <main class="pb-12 pt-6 lg:pt-10">
      <RouterView />
    </main>
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
</script>