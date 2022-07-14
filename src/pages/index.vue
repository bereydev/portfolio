<script setup lang="ts">
const { t } = useI18n()
</script>

<!-- <template>
  <div>
    <p>
      <a rel="noreferrer" class="text-4xl " href="https://github.com/bereydev" target="_blank">
        Bereyziat Development
      </a>
    </p>
    <p>
      <em class="text-sm opacity-75">{{ t('intro.desc') }}</em>
    </p>
    <p class="text-xl opacity-80">
      {{ t('intro.coming-soon') }}
    </p>
  </div>
</template> -->

<template>
  <!-- Section 1 -->
  <NavBar />

  <!-- Section 2 -->
  <section class="px-2 py-10 md:py-32 bg-white md:px-0">
    <div class="container items-center max-w-6xl px-8 mx-auto xl:px-5">
      <div class="flex flex-wrap items-center sm:-mx-3">
        <div class="w-full md:w-1/2 md:px-3">
          <div
            class="w-full pb-6 space-y-6 sm:max-w-md lg:max-w-lg md:space-y-4 lg:space-y-8 xl:space-y-9 sm:pr-5 lg:pr-0 md:pb-0"
          >
            <h1
              class="text-4xl font-extrabold tracking-tight text-gray-900 sm:text-5xl md:text-4xl lg:text-5xl xl:text-6xl"
            >
              <span class="block xl:inline">{{ t('hero.title_1') }}<p /></span>
              <span class="block gradient-title xl:inline">{{ t('hero.title_2') }}</span>
            </h1>
            <p class="mx-auto text-base text-2xl text-gray-500 sm:max-w-md md:max-w-3xl">
              {{ t('hero.desc') }}
            </p>
            <div class="relative flex flex-col sm:flex-row sm:space-x-4">
              <a
                href="https://calendly.com/bereydev" target="_blank"
                class="flex items-center w-full px-6 py-3 mb-3 text-lg text-white bg-purple-500 rounded-full sm:mb-0 hover:bg-purple-700 sm:w-auto"
              >
                {{ t('button.talk') }}
              </a>
              <a
                href="mailto:contact@bereyziat.dev"
                class="flex items-center px-6 py-3 text-lg text-gray-500 bg-gray-100 rounded-full hover:bg-gray-200 hover:text-gray-600"
              >
                {{ t('button.send_mail') }}
              </a>
            </div>
          </div>
        </div>
        <div class="w-full md:w-1/2">
          <div class="w-full h-auto overflow-hidden rounded-md shadow-xl sm:rounded-xl">
            <img
              src="https://images.unsplash.com/photo-1498049860654-af1a5c566876?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1050&q=80"
            >
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Section 3 -->
  <section class="w-full bg-white pt-7 pb-7 md:pt-20 md:pb-24">
    <div
      class="box-border flex flex-col items-center content-center mb-20 sm:mb-40 px-8 mx-auto leading-6 text-black border-0 border-gray-300 border-solid md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-5 mb-4 -ml-5 text-center bg-no-repeat bg-contain border-solid md:ml-0 md:mt-0 md:max-w-none lg:mb-0 md:w-1/2 xl:pl-10"
      >
        <img
          src="/brainstorming.svg"
          class="p-2 pl-6 pr-5 xl:pl-16 xl:pr-20 "
        >
      </div>

      <!-- Content -->
      <div class="box-border order-first w-full text-black border-solid md:w-1/2 md:pl-10 md:order-none">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          {{ t('brainstorm.title_1') }} <br> {{ t('brainstorm.title_2') }}
        </h2>
        <p class="pt-4 pb-8 m-0 leading-7 text-gray-700 border-0 text-2xl border-gray-300 sm:pr-12 xl:pr-32">
          {{ t('brainstorm.desc_1') }} <br>{{ t('brainstorm.desc_2') }}
        </p>
      </div>
      <!-- End  Content -->
    </div>
    <div
      class="box-border flex flex-col items-center content-center mb-20 sm:mb-40 px-8 mx-auto mt-2 leading-6 text-black border-0 border-gray-300 border-solid md:mt-20 xl:mt-0 md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Content -->
      <div class="box-border w-full text-black border-solid md:w-1/2 md:pl-6 xl:pl-32">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          {{ t('plan.title') }}
        </h2>
        <ul class="p-0 m-0 pt-4 leading-6 border-0 border-gray-300">
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">{{ t('plan.bullet_1') }}</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">{{ t('plan.bullet_2') }}</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">{{ t('plan.bullet_3') }}</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">{{ t('plan.bullet_4') }}</span>
          </li>
        </ul>
      </div>
      <!-- End  Content -->

      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-10 mb-20 sm:mb-40 text-center bg-no-repeat bg-contain border-solid md:mt-0 md:max-w-none lg:mb-0 md:w-1/2"
      >
        <img src="/planning.svg" class="pl-4 sm:pr-10 xl:pl-10 lg:pr-32">
      </div>
    </div>
    <div
      class="box-border flex flex-col items-center content-center px-8 mx-auto leading-6 mb-4 text-black border-0 border-gray-300 border-solid md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-5 mb-4 -ml-5 text-center bg-no-repeat bg-contain border-solid md:ml-0 md:mt-0 md:max-w-none lg:mb-0 md:w-1/2 xl:pl-10"
      >
        <img
          src="/launching.svg"
          class="p-2 pl-6 pr-5 xl:pl-16 xl:pr-20 "
        >
      </div>

      <!-- Content -->
      <div class="box-border order-first w-full text-black border-solid md:w-1/2 md:pl-10 md:order-none">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          {{ t('launch.title') }}
        </h2>
        <p class="pt-4 pb-8 m-0 leading-7 text-gray-700 border-0 text-2xl border-gray-300 sm:pr-12 xl:pr-32">
          {{ t('launch.desc_1') }}<br>
          {{ t('launch.desc_2') }}
        </p>
      </div>
      <!-- End  Content -->
    </div>
  </section>
  <section class="bg-white">
    <div class="container flex flex-row justify-center items-center max-w-6xl px-8 mx-auto xl:px-5">
      <a
        href="https://calendly.com/bereydev" target="_blank"
        class="flex items-center w-full px-6 py-3 mb-3 text-lg text-white bg-purple-500 rounded-full sm:mb-0 hover:bg-purple-700 sm:w-auto"
      >
        {{ t('button.book_meeting') }}
      </a>
    </div>
  </section>

  <FooterSection />
</template>

<route lang="yaml">
meta:
  layout: none
</route>
