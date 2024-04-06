<script setup lang="ts">
  import moneyFaceLogo from "@/assets/images/money-face-icon.png"
</script>

<template>
  <header class="w-full shadow">
    <nav class="bg-white px-4 lg:px-6 py-2.5">
      <div class="flex justify-center md:justify-between items-center mx-auto max-w-screen-xl">
        <div class="flex items-center">
          <img :src="moneyFaceLogo" alt="logo do money face" class="max-w-7 mr-2"> 
          <p class="text-lg">
            Money Face
          </p>
        </div>
      </div>
    </nav>
  </header>
</template>
