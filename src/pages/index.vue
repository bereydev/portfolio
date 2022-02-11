<script setup lang="ts">
const { t } = useI18n()
</script>

<template>
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
</template>
