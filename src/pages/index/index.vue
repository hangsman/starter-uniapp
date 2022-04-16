<script setup lang="ts">
import HelloWord from '@/components/HelloWord.vue'
import { useCounterStore } from '@/stores/counter'

const countStore = useCounterStore()
const { increment } = useCounterStore()

</script>

<template>
  <div class="flex flex-col items-center justify-center">
    <img class="h-200rpx w-200rpx mt-200rpx mx-auto mb-50rpx" src="@/static/logo.png" alt="">
    <div class="flex justify-center items-center flex-col">
      <span class="text-36rpx text-hex-8f8f94">
        {{ countStore.count }}
      </span>
      <button class="mt-20rpx px-35rpx py-15rpx bg-blue-400 text-white font-medium text-xs uppercase rounded shadow-md" @click="increment()">
        add
      </button>
      <HelloWord title="title"/>
    </div>
  </div>
</template>
