<script setup lang="ts">

const { t, availableLocales, locale } = useI18n()
const locales = availableLocales

locale.value = availableLocales.includes(navigator.language) ? navigator.language : 'en'

const toggleLocales = () => {
  // change to some real logic
  locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
}

</script>

<template>
  <section class="w-full px-8 text-gray-700 bg-white">
    <div class="container flex flex-col flex-wrap items-center justify-between py-5 mx-auto md:flex-row max-w-7xl">
      <div class="relative flex items-center justify-between w-full md:w-auto flex-row">
        <a
          href="#_"
          class="flex items-center mb-0 font-medium text-gray-900 lg:w-auto lg:items-center lg:justify-center"
        >
          <span class="mx-auto text-xl font-black leading-none text-gray-900 select-none">
            <img src="/bereyziat_logo_full.svg" height="60" width="200" alt="Bereyziat Development Logo">
          </span>
        </a>
        <!-- <nav class="flex flex-wrap items-center mb-5 text-base md:mb-0 md:pl-8 md:ml-8 md:border-l md:border-gray-200">
          <a href="#_" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900">Home</a>
          <a href="#_" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900">Features</a>
          <a href="#_" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900">Pricing</a>
          <a href="#_" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900">Blog</a>
        </nav> -->
        <a
          href="#"
          class="text-base font-medium leading-6 text-gray-600 whitespace-no-wrap transition duration-150 ease-in-out block md:hidden hover:text-gray-900"
          @click="toggleLocales"
        >
          {{ locales[(locales.indexOf(locale) + 1) % locales.length].toUpperCase() }}
        </a>
      </div>

      <div class="inline-flex items-center ml-5 space-x-6 hidden md:block lg:justify-end">
        <a
          href="#"
          class="text-base font-medium leading-6 text-gray-600 whitespace-no-wrap transition duration-150 ease-in-out hover:text-gray-900"
          @click="toggleLocales"
        >
          {{ locales[(locales.indexOf(locale) + 1) % locales.length].toUpperCase() }}
        </a>

        <a
          href="mailto:contact@bereyziat.dev"
          class="inline-flex items-center justify-center px-4 py-2 text-base font-medium leading-6 text-white whitespace-no-wrap bg-purple-500 border border-transparent rounded-full shadow-sm hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-600"
        >
          {{ t('button.contact') }}
        </a>
      </div>
    </div>
  </section>
</template>
