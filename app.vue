<template>
  <div>
    <ClientOnly>
      <IronManWelcome />
      <template #fallback>
        <p class="my-6 flex justify-center">[IronManWelcome] 載入中...</p>
      </template>
    </ClientOnly>
  </div>
</template>

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
