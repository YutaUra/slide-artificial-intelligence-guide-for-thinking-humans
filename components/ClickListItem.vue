<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  click: {
    type: Number,
    required: true,
  },
})
</script>

<template>
  <div
    v-if="$slidev.nav.clicks >= click"
    v-motion
    :initial="{ x: -40, y: 10, opacity: 0 }"
    :enter="{ x: 0, y: 0, opacity: 1, transition: { duration: 800 } }"
  >
    <mdi-arrow-right class="inline" /> <slot />
  </div>
</template>
