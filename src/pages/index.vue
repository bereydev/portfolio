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
  <section class="px-2 py-32 bg-white md:px-0">
    <div class="container items-center max-w-6xl px-8 mx-auto xl:px-5">
      <div class="flex flex-wrap items-center sm:-mx-3">
        <div class="w-full md:w-1/2 md:px-3">
          <div
            class="w-full pb-6 space-y-6 sm:max-w-md lg:max-w-lg md:space-y-4 lg:space-y-8 xl:space-y-9 sm:pr-5 lg:pr-0 md:pb-0"
          >
            <h1
              class="text-4xl font-extrabold tracking-tight text-gray-900 sm:text-5xl md:text-4xl lg:text-5xl xl:text-6xl"
            >
              <span class="block xl:inline">Tell us what you need and</span>
              <span class="block text-indigo-600 xl:inline"> watch your idea come to life </span>
            </h1>
            <p class="mx-auto text-base text-gray-500 sm:max-w-md lg:text-xl md:max-w-3xl">
              With our agile team of developers, we help you to develop your projects with the most advanced tech and fist-class business advices.
            </p>
            <div class="relative flex flex-col sm:flex-row sm:space-x-4">
              <a
                href="https://calendly.com/bereydev"
                class="flex items-center w-full px-6 py-3 mb-3 text-lg text-white bg-indigo-600 rounded-full sm:mb-0 hover:bg-indigo-700 sm:w-auto"
              >
                Let's talk
              </a>
              <a
                href="mailto:contact@bereyziat.dev"
                class="flex items-center px-6 py-3 text-gray-500 bg-gray-100 rounded-full hover:bg-gray-200 hover:text-gray-600"
              >
                Send us an email
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
      class="box-border flex flex-col items-center content-center px-8 mx-auto leading-6 text-black border-0 border-gray-300 border-solid md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-5 mb-4 -ml-5 text-center bg-no-repeat bg-contain border-solid md:ml-0 md:mt-0 md:max-w-none lg:mb-0 md:w-1/2 xl:pl-10"
      >
        <img
          src="https://cdn.devdojo.com/images/december2020/productivity.png"
          class="p-2 pl-6 pr-5 xl:pl-16 xl:pr-20 "
        >
      </div>

      <!-- Content -->
      <div class="box-border order-first w-full text-black border-solid md:w-1/2 md:pl-10 md:order-none">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          Brainstorm <br> with our engineers
        </h2>
        <p class="pt-4 pb-8 m-0 leading-7 text-gray-700 border-0 border-gray-300 sm:pr-12 xl:pr-32 lg:text-2xl">
          Let's build together a strategic approach to your project in a creative atmosphere. <br>Our young team makes cool look easy.
        </p>
      </div>
      <!-- End  Content -->
    </div>
    <div
      class="box-border flex flex-col items-center content-center px-8 mx-auto mt-2 leading-6 text-black border-0 border-gray-300 border-solid md:mt-20 xl:mt-0 md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Content -->
      <div class="box-border w-full text-black border-solid md:w-1/2 md:pl-6 xl:pl-32">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          Design a product plan
        </h2>
        <ul class="p-0 m-0 pt-4 leading-6 border-0 border-gray-300">
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">We help you decide what tech would fit the best your needs</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">We define the steps to succeed with your idea</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">We define together a timeframe and a budget</span>
          </li>
          <li class="box-border relative py-1 pl-0 text-left text-gray-500 border-solid">
            <span
              class="inline-flex items-center justify-center w-6 h-6 mr-2 text-white bg-purple-500 rounded-full"
            ><span
              class="text-sm font-bold"
            >✓</span></span> <span class="text-2xl">We provide you with a free mock-up preview</span>
          </li>
        </ul>
      </div>
      <!-- End  Content -->

      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-10 mb-4 text-center bg-no-repeat bg-contain border-solid md:mt-0 md:max-w-none lg:mb-0 md:w-1/2"
      >
        <img src="https://cdn.devdojo.com/images/december2020/settings.png" class="pl-4 sm:pr-10 xl:pl-10 lg:pr-32">
      </div>
    </div>
    <div
      class="box-border flex flex-col items-center content-center px-8 mx-auto leading-6 text-black border-0 border-gray-300 border-solid md:flex-row max-w-7xl lg:px-16"
    >
      <!-- Image -->
      <div
        class="box-border relative w-full max-w-md px-4 mt-5 mb-4 -ml-5 text-center bg-no-repeat bg-contain border-solid md:ml-0 md:mt-0 md:max-w-none lg:mb-0 md:w-1/2 xl:pl-10"
      >
        <img
          src="https://cdn.devdojo.com/images/december2020/productivity.png"
          class="p-2 pl-6 pr-5 xl:pl-16 xl:pr-20 "
        >
      </div>

      <!-- Content -->
      <div class="box-border order-first w-full text-black border-solid md:w-1/2 md:pl-10 md:order-none">
        <h2 class="m-0 text-3xl font-semibold leading-tight border-0 border-gray-300 lg:text-5xl md:text-4xl">
          Make it happen
        </h2>
        <p class="pt-4 pb-8 m-0 leading-7 text-gray-700 border-0 border-gray-300 sm:pr-12 xl:pr-32 lg:text-2xl">
          Build an atmosphere that creates productivity in your organization and your company culture.
        </p>
      </div>
      <!-- End  Content -->
    </div>
  </section>

  <FooterSection />
</template>

<route lang="yaml">
meta:
  layout: none
</route>
