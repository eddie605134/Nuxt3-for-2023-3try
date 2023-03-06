<template>
  <!-- <div class="py-24 bg-white">
    <div class="flex justify-center">
      <Icon name="logos:nuxt" size="360" />
    </div>
    <div class="flex flex-col items-center">
      <h1 class="my-2 text-6xl font-semibold text-sky-400">{{ title }}</h1>
      <h1 class="my-2 text-6xl font-semibold text-emerald-400">{{ $hello('Jennifer') }}</h1>
    </div>
    <div class="flex justify-center">
      <button
        v-focus
        class="w-[100px] border-t-neutral-50 bg-slate-600 text-neutral-700 focus:text-white"
      >
        測試
      </button>
    </div>
  </div> -->
  <NuxtPage />
</template>

<script lang="ts" setup>
const { $hello } = useNuxtApp()
const title = $hello('Ryan')
</script>

<!-- <template>
  <div class="flex flex-col items-center">
    <div class="flex items-center mt-8">
      <input
        id="show-button"
        v-model="useRound"
        name="show-button"
        type="checkbox"
        class="w-5 h-5"
      />
      <label for="show-button" class="block ml-2 text-base text-slate-800">使用圓角按鈕</label>
    </div>
    <component :is="useRound ? RoundButton : BaseButton" />
  </div>
</template>

<script lang="ts" setup>
const useRound = ref(false)
// 加 Lazy 前墜會變成動態載入
const BaseButton = resolveComponent('LazyBaseApplyButton')
const RoundButton = resolveComponent('LazyRoundApplyButton')
</script> -->
