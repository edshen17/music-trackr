<script setup lang="ts">
import { toggleDark } from '~/composables'

const { t } = useI18n()

</script>

<template>
  <footer>
    <div class="border border-t-2 border-gray-200 dark:border-transparent">
      <div class="container px-5 py-6 mx-auto flex items-center sm:flex-row flex-col">
        <p class="sm:ml-6 sm:mt-0 mt-4">
          {{ t('copyright') }}
        </p>
        <span class="inline-flex sm:ml-auto sm:mt-0 mt-4 justify-center sm:justify-start">
          <button class="icon-btn mx-2" @click="toggleDark()">
            <div i="carbon-sun dark:carbon-moon" class="text-2xl" />
          </button>
        </span>
      </div>
    </div>
  </footer>
</template>
