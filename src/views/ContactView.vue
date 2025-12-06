<template>
  <section class="mx-auto max-w-4xl px-4 lg:px-6">
    <header class="mb-6 lg:mb-8">
      <h1 class="text-2xl font-semibold italic text-slate-900 lg:text-3xl">
        Get In Touch
      </h1>
      <p class="mt-2 text-sm text-slate-600 lg:text-base">
        I’m open to collaboration, part-time roles, and full-time full-stack
        opportunities.
      </p>
    </header>

    <div
      class="space-y-6 rounded-2xl bg-white p-6 shadow-sm ring-1 ring-slate-200 lg:p-8"
    >
      <!-- Contact info（可点击） -->
      <div class="rounded-2xl bg-slate-50 p-4 text-sm text-slate-800 space-y-1">
        <p>
          Email ·
          <a
            href="mailto:wcer.my@gmail.com"
            class="text-blue-600 hover:underline"
          >
            wcer.my@gmail.com
          </a>
        </p>

        <p>
          GitHub ·
          <a
            href="https://github.com/Micrasoft007"
            target="_blank"
            rel="noopener"
            class="text-blue-600 hover:underline"
          >
            github.com/Micrasoft007
          </a>
        </p>

        <p>
          LinkedIn ·
          <a
            href="https://ca.linkedin.com/in/zexi-wang-91311123b"
            target="_blank"
            rel="noopener"
            class="text-blue-600 hover:underline"
          >
            Zexi Wang
          </a>
        </p>
      </div>

      <!-- Message 区域 -->
      <form class="space-y-4" @submit.prevent="sendMail">
        <textarea
          rows="4"
          v-model="message"
          placeholder="Message"
          class="w-full rounded-2xl border border-slate-200 bg-slate-50 px-4 py-3 text-sm outline-none focus:bg-white focus:ring-2 focus:ring-blue-300"
        />

        <button
          type="submit"
          class="inline-flex rounded-full bg-blue-500 px-6 py-2 text-sm font-medium text-white shadow-sm hover:bg-blue-600"
        >
          Send Message
        </button>
      </form>

      <p class="text-xs text-slate-500">
        Looking forward to connecting with you!
      </p>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const message = ref('');

const sendMail = () => {
  const body = encodeURIComponent(message.value || '');
  const subject = encodeURIComponent('Portfolio Contact');
  window.location.href = `mailto:wcer.my@gmail.com?subject=${subject}&body=${body}`;
};
</script>