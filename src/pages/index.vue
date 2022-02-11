<script setup lang="ts">
import { useUserStore } from '~/stores/user'

const user = useUserStore()
const name = ref(user.savedName)

const router = useRouter()
const go = () => {
  if (name.value)
    router.push(`/hi/${encodeURIComponent(name.value)}`)
}

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

    <div class="py-4" />
  </div>
</template>
