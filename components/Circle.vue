<!--
Circle
<circle x="10" y="20" r="30" color="green" width="3" />
<circle v-bind="{ x:10, y:10, r:200 }"/>
-->

<script setup lang="ts">
import { defineProps } from 'vue'
import { customAlphabet } from 'nanoid'

const nanoid = customAlphabet('abcedfghicklmn', 10)

defineProps<{
  x: number | string
  y: number | string
  r: number | string
  width?: number | string
  color?: string
}>()
</script>

<template>
  <svg
    class="absolute left-0 top-0 pointer-events-none"
    :width="Math.max(+x + +r) + +(width || 1) + 5"
    :height="Math.max(+y + +r) + +(width || 1) + 5"
  >
    <circle
      :cx="+x"
      :cy="+y"
      :r="+r"
      :stroke="color"
      :stroke-width="width || 1"
      fill="none"
    />
  </svg>
</template>
