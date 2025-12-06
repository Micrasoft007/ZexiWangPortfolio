<template>
  <header class="bg-slate-800 text-white">
    <nav
      class="mx-auto flex max-w-6xl items-center justify-between px-4 py-4 lg:px-6"
    >
      <RouterLink to="/about" class="font-medium tracking-tight">
        Zexi Wang · Full Stack Developer
      </RouterLink>

      <!-- Desktop nav -->
      <div class="hidden gap-8 text-sm font-medium lg:flex">
        <RouterLink
          v-for="item in navItems"
          :key="item.to"
          :to="item.to"
          class="transition-colors"
          :class="
            route.name === item.name
              ? 'text-white'
              : 'text-slate-200 hover:text-white'
          "
        >
          {{ item.label }}
        </RouterLink>
      </div>

      <!-- Mobile hamburger -->
      <button
        class="flex flex-col items-center justify-center space-y-1.5 rounded-md p-2 hover:bg-slate-700 lg:hidden"
        @click="open = !open"
        aria-label="Open menu"
      >
        <span
          class="block h-0.5 w-5 bg-white transition"
          :class="open ? 'translate-y-2 rotate-45' : ''"
        ></span>
        <span
          class="block h-0.5 w-5 bg-white transition"
          :class="open ? 'opacity-0' : ''"
        ></span>
        <span
          class="block h-0.5 w-5 bg-white transition"
          :class="open ? '-translate-y-2 -rotate-45' : ''"
        ></span>
      </button>
    </nav>

    <!-- Mobile menu overlay -->
    <transition name="fade">
      <div
        v-if="open"
        class="fixed inset-0 z-40 bg-black/40 lg:hidden"
        @click.self="open = false"
      >
        <aside class="h-full w-64 bg-white pt-4 shadow-xl">
          <div class="px-4 pb-4">
            <p class="text-base font-semibold text-slate-800">Menu</p>
          </div>
          <nav class="space-y-1">
            <button
              v-for="item in navItems"
              :key="item.to"
              @click="go(item.to)"
              class="block w-full px-4 py-2 text-left text-sm font-medium"
              :class="
                route.name === item.name
                  ? 'bg-slate-100 text-slate-900'
                  : 'text-slate-700 hover:bg-slate-50'
              "
            >
              {{ item.label }}
            </button>
          </nav>
          <p class="px-4 pt-6 text-xs text-slate-400">
            Tap outside to close
          </p>
        </aside>
      </div>
    </transition>
  </header>
</template>

<script setup>
import { RouterLink, useRoute, useRouter } from 'vue-router';
import { ref } from 'vue';

const route = useRoute();
const router = useRouter();
const open = ref(false);

const navItems = [
  { label: 'About', to: '/about', name: 'about' },
  { label: 'Projects', to: '/projects', name: 'projects' },
  { label: 'Contact', to: '/contact', name: 'contact' },
];

function go(path) {
  router.push(path);
  open.value = false;
}
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.18s ease-out;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>