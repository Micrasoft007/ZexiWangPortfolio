<template>
  <section class="mx-auto max-w-6xl px-4 lg:px-6">
    <header class="mb-6 lg:mb-8">
      <h1 class="text-2xl font-semibold text-slate-900 lg:text-3xl">
        Highlighted Projects
      </h1>
      <p class="mt-2 text-sm text-slate-600 lg:text-base">
        A selection of logistics, e-commerce, and automation work.
      </p>
    </header>

    <div class="grid gap-6 lg:grid-cols-2">
      <!-- Lulugo -->
      <article
        class="flex h-full flex-col justify-between rounded-2xl bg-white p-5 shadow-sm ring-1 ring-slate-200"
      >
        <div>
          <h2 class="text-base font-semibold text-slate-900">
            Lulugo – Intelligent Logistics Management Platform
          </h2>
          <p class="mt-2 text-sm text-slate-600">
            Cross-platform Flutter app + Django backend for drivers and
            logistics companies. AI video &amp; photo OCR imports orders; Google
            OR-Tools optimizes routes; real-time driver tracking, attendance,
            and multi-tenant company separation.
          </p>
          <div class="mt-3 flex flex-wrap gap-2">
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Flutter
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Django
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              OpenAI Vision
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              OR-Tools
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              PostgreSQL
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Docker
            </span>
          </div>
        </div>

        <!-- Lulugo 按钮：Web + iOS + Android -->
        <div class="mt-4 flex flex-wrap gap-3">
          <a
            href="https://admin.lulugo.tech/"
            target="_blank"
            rel="noreferrer"
            class="inline-flex items-center justify-center rounded-lg bg-blue-500 px-4 py-2 text-xs font-medium text-white hover:bg-blue-600"
          >
            View admin web
          </a>
          <a
            href="https://apps.apple.com/ca/app/lulugo/id6745342904"
            target="_blank"
            rel="noreferrer"
            class="inline-flex items-center justify-center rounded-lg bg-slate-900 px-4 py-2 text-xs font-medium text-white hover:bg-slate-950"
          >
            iOS App
          </a>
          <a
            href="https://appdistribution.firebase.google.com/pub/i/02bf42563ac90cb5"
            target="_blank"
            rel="noreferrer"
            class="inline-flex items-center justify-center rounded-lg bg-emerald-500 px-4 py-2 text-xs font-medium text-white hover:bg-emerald-600"
          >
            Android App
          </a>
        </div>
      </article>

      <!-- SuperRoute Shopify app -->
      <article
        class="flex h-full flex-col justify-between rounded-2xl bg-white p-5 shadow-sm ring-1 ring-slate-200"
      >
        <div>
          <h2 class="text-base font-semibold text-slate-900">
            SuperRoute – Shopify Courier Label App
          </h2>
          <p class="mt-2 text-sm text-slate-600">
            Shopify app that imports orders in real time, generates courier
            labels, and automates shipping workflows. Built with Node.js,
            Shopify Polaris UI, and deployed on Linux servers with performance
            tuning.
          </p>
          <div class="mt-3 flex flex-wrap gap-2">
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Node.js
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Shopify
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Polaris
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              SQLite
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Linux
            </span>
          </div>
        </div>

        <a
          href="https://apps.shopify.com/fleetexpress?search_id=fb405ad1-c482-4f6e-a336-eda968812bf8&surface_detail=superroute&surface_inter_position=1&surface_intra_position=1&surface_type=search"
          target="_blank"
          rel="noreferrer"
          class="mt-4 inline-flex w-max items-center justify-center rounded-lg bg-blue-500 px-4 py-2 text-xs font-medium text-white hover:bg-blue-600"
        >
          View on Shopify App Store
        </a>
      </article>

      <!-- Smart Inventory Sync -->
      <article
        class="flex h-full flex-col justify-between rounded-2xl bg-white p-5 shadow-sm ring-1 ring-slate-200 lg:col-span-2"
      >
        <div>
          <h2 class="text-base font-semibold text-slate-900">
            Smart Inventory Sync System
          </h2>
          <p class="mt-2 text-sm text-slate-600">
            Backend system using Odoo 19 to integrate Shopify, eBay, Temu,
            TikTok, and Walmart. Syncs inventory, imports orders, handles bulk
            file uploads, and automates label printing through SuperRoute.
          </p>
          <div class="mt-3 flex flex-wrap gap-2">
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Odoo 16
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              PostgreSQL
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              APIs
            </span>
            <span
              class="inline-flex items-center rounded-full bg-slate-100 px-3 py-1 text-xs font-medium text-slate-700"
            >
              Multi-channel
            </span>
          </div>
        </div>

        <a
          href="http://66.70.176.224:8069/odoo/inventory"
          target="_blank"
          rel="noreferrer"
          class="mt-4 inline-flex w-max items-center justify-center rounded-lg bg-blue-500 px-4 py-2 text-xs font-medium text-white hover:bg-blue-600"
        >
          View live demo
        </a>
      </article>
    </div>
  </section>
</template>