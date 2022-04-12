<script setup lang="ts">
import { ref } from 'vue'
const title = ref('Hello')
</script>

<template>
  <div class="flex flex-col items-center justify-center">
    <img class="h-200rpx w-200rpx mt-200rpx mx-auto mb-50rpx" src="/static/logo.png">
    <div class="flex justify-center">
      <span class="text-36rpx text-hex-8f8f94">
        {{ title }}
      </span>
    </div>
  </div>
</template>
