<script setup lang="ts">
import { ref } from 'vue'
import { useCounterStore } from '@/stores/counter'
const title = ref('Hello')

const countStore = useCounterStore()
const { increment } = useCounterStore()
</script>

<template>
  <div class="flex flex-col items-center justify-center">
    <img class="h-200rpx w-200rpx mt-200rpx mx-auto mb-50rpx" src="/static/logo.png">
    <div class="flex justify-center items-center flex-col">
      <span class="text-36rpx text-hex-8f8f94">
        {{ countStore.count }}
      </span>
      <button class="mt-20rpx" @click="increment()">
        add
      </button>
    </div>
  </div>
</template>
