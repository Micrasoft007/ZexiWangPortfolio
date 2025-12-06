<template>
  <section class="mx-auto max-w-6xl px-4 lg:px-6">
    <!-- Hero + Focus -->
    <div
      class="grid gap-6 lg:grid-cols-[minmax(0,1.4fr)_minmax(0,1fr)] lg:items-stretch"
    >
      <!-- Hero card -->
      <div
        class="rounded-2xl bg-white p-6 shadow-sm ring-1 ring-slate-200 lg:p-8"
      >
        <h1 class="text-2xl font-semibold text-slate-900 lg:text-3xl">
          Hi, I'm Zexi.
        </h1>
        <p class="mt-3 text-sm leading-relaxed text-slate-600 lg:text-base">
          Full stack development student and part-time developer specializing in
          Flutter, Django, and AI-powered systems.
        </p>
        <p class="mt-2 text-sm leading-relaxed text-slate-600 lg:text-base">
          I build mobile apps, backend services, and automation workflows that
          connect logistics, e-commerce, and data.
        </p>

        <div class="mt-6 flex flex-wrap gap-3">
          <RouterLink
            to="/projects"
            class="inline-flex items-center justify-center rounded-lg bg-blue-500 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-blue-600"
          >
            View Projects
          </RouterLink>
          <a
            href="/Zexi-Wang-CV.pdf"
            download
            class="inline-flex items-center justify-center rounded-lg border border-slate-300 bg-white px-4 py-2 text-sm font-medium text-slate-700 hover:bg-slate-50"
          >
            Download CV
          </a>
        </div>
      </div>

      <!-- Focus card -->
      <div
        class="flex items-center justify-center rounded-2xl bg-slate-800 px-6 py-10 lg:px-10"
      >
        <div class="relative h-48 w-full max-w-sm">
          <div
            class="absolute right-6 top-1/2 -translate-y-1/6 mt-18 text-right"
          >
            <p class="text-sm font-semibold text-slate-200">Focus:</p>
            <p class="mt-1 text-sm text-slate-100">
              Logistics · E-commerce · AI Automation
            </p>
          </div>
          <div class="absolute -left-4 top-10 h-20 w-20 rounded-full bg-slate-100"></div>
          <div class="absolute left-12 top-4 h-40 w-40 rounded-full bg-blue-500/80"></div>
        </div>
      </div>
    </div>
Download CV
    <!-- 下半部分：先 Skills，再 Education + Experience 两列 -->
    <div class="mt-10 space-y-10">
      <!-- Skills 全宽 -->
      <section>
        <h2 class="text-xl font-semibold text-slate-900">Skills</h2>

        <div class="mt-4 grid gap-4 md:grid-cols-2">
          <article
            class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
          >
            <h3 class="text-sm font-semibold text-slate-900">Frontend</h3>
            <p class="mt-2 text-sm text-slate-600">
              Flutter · Dart<br />
              React<br />
              Responsive UI · Figma
            </p>
          </article>

          <article
            class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
          >
            <h3 class="text-sm font-semibold text-slate-900">Backend</h3>
            <p class="mt-2 text-sm text-slate-600">
              Django · Python<br />
              Node.js · Odoo<br />
              REST APIs
            </p>
          </article>

          <article
            class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
          >
            <h3 class="text-sm font-semibold text-slate-900">Databases</h3>
            <p class="mt-2 text-sm text-slate-600">
              PostgreSQL · SQLite · MongoDB<br />
              Query optimization
            </p>
          </article>

          <article
            class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
          >
            <h3 class="text-sm font-semibold text-slate-900">DevOps</h3>
            <p class="mt-2 text-sm text-slate-600">
              Docker · Linux server<br />
              CI/CD basics<br />
              Celery · Redis
            </p>
          </article>
        </div>

        <article
          class="mt-4 rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
        >
          <h3 class="text-sm font-semibold text-slate-900">AI & APIs</h3>
          <p class="mt-2 text-sm text-slate-600">
            OpenAI Vision & GPT models · Google Maps / Geocoding / OR-Tools ·
            Shopify · Odoo 16 · multi-channel e-commerce integrations.
          </p>
        </article>
      </section>

      <!-- Education + Experience 两列 -->
      <section
        class="grid gap-8 lg:grid-cols-2 lg:items-start"
      >
        <!-- Education -->
        <div>
          <h2 class="text-xl font-semibold text-slate-900">Education</h2>
          <div class="mt-4 space-y-3">
            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Nova Scotia Community College (NSCC)
              </p>
              <p class="mt-1 text-xs text-slate-600">
                Postgraduate · Computer Programming · Grade 95%
              </p>
              <p class="mt-1 text-xs text-slate-500">
                2025 – 2026 · Full-stack development focus.
              </p>
            </div>

            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                George Brown College
              </p>
              <p class="mt-1 text-xs text-slate-600">
                Mobile Application Development & Strategy · Grade 95%
              </p>
              <p class="mt-1 text-xs text-slate-500">
                2024 – 2025 · App architecture, UX/UI, cross-platform.
              </p>
            </div>

            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Hubei Normal University
              </p>
              <p class="mt-1 text-xs text-slate-600">
                B.Eng. Communication Engineering · Grade 85%
              </p>
              <p class="mt-1 text-xs text-slate-500">
                2017 – 2021 · C / Java / SQL / data structures.
              </p>
            </div>
          </div>
        </div>

        <!-- Experience -->
        <div>
          <h2 class="text-xl font-semibold text-slate-900">Experience</h2>
          <div class="mt-4 space-y-3">
            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Chief Technology Officer · Lulugo Tech
              </p>
              <p class="mt-1 text-xs text-slate-600">2025 – Present · Remote</p>
              <p class="mt-1 text-xs text-slate-500">
                Leading development of Lulugo logistics platform using Flutter +
                Django.
              </p>
            </div>

            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Shopify App Developer · Superroute Inc.
              </p>
              <p class="mt-1 text-xs text-slate-600">2024 – Present · Remote</p>
              <p class="mt-1 text-xs text-slate-500">
                Building courier label automation apps for Shopify merchants.
              </p>
            </div>

            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Odoo Developer · Syminno
              </p>
              <p class="mt-1 text-xs text-slate-600">2024 – Present · Remote</p>
              <p class="mt-1 text-xs text-slate-500">
                Integrating Odoo 16 with multi-channel e-commerce platforms.
              </p>
            </div>

            <div
              class="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-slate-200"
            >
              <p class="text-sm font-semibold text-slate-900">
                Odoo Backend Developer · Karrytech
              </p>
              <p class="mt-1 text-xs text-slate-600">
                2021 – 2023 · Wuhan · On-site
              </p>
              <p class="mt-1 text-xs text-slate-500">
                Implemented HRP modules, reports, and REST/XML integrations.
              </p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </section>
</template>