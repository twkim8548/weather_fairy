<script setup lang="ts">
import { Vue3Lottie } from 'vue3-lottie'
import PartyJson from '/src/assets/json/Party.json'
</script>

<template>
  <div class="flex flex-col items-center justify-center overflow-hidden">
    <Vue3Lottie
        :animationData="PartyJson"
        :height="300"
        :width="380"
        :speed="0.8"
        :loop="false"
        class="overflow-hidden"
        @on-complete="$router.replace('/main')"
    />
    <p class="text-4xl absolute animate-[fade_1s_ease-in-out] text-center  font-[HSSanTokki20-Regular]">
      출퇴근길
      <br>
      날씨요정
    </p>
  </div>
</template>