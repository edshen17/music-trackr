<script setup lang="ts">
const { t } = useI18n()
</script>

<template>
  <div>
    {{ t('notFound') }}
  </div>
</template>

<route lang="yaml">
meta:
  layout: 404
</route>