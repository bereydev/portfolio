<script setup lang="ts">
const { t, availableLocales, locale } = useI18n()
const locales = availableLocales

locale.value = availableLocales.includes(navigator.language) ? navigator.language : 'en'

const setLocale = (value: string) => {
  // change to some real logic
  locale.value = value
//   isVisible.value = false
}

</script>

<template>
  <div class=" relative inline-block text-left dropdown">
    <span class="rounded-md shadow-sm">
      <button
        class="inline-flex justify-center w-full px-4 py-2 text-sm font-medium leading-5 text-gray-600 transition duration-150 ease-in-out bg-white rounded-md font-medium hover:text-gray-900"
        type="button"
        aria-haspopup="true" aria-expanded="true" aria-controls="language-menu"
      >
        <span>{{ locale.toUpperCase() }}</span>

        <svg class="w-5 h-5 ml-2 -mr-1" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" /></svg>

      </button></span>
    <div class="opacity-0 invisble dropdown-menu transition-all duration-300 transform origin-top-right -translate-y-2 scale-95">
      <div id="language-menu" class="absolute right-0 origin-top-right bg-white divide-y rounded-md shadow-lg outline-none p-2" aria-labelledby="headlessui-menu-button-1" role="menu">
        <div class="py-3">
          <div v-for="l, index in locales" :key="l">
            <a href="javascript:void(0)" tabindex="{{index}}" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left" role="menuitem" @click="setLocale(l)">
              {{ l.toUpperCase() }}
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.dropdown:focus-within .dropdown-menu {
  opacity:1;
  transform: translate(0) scale(1);
  visibility: visible;
}
</style>
