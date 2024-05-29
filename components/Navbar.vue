<template>
  <UContainer as="section">
    <div>
<nav class="shadow-xl">
  <div class="flex justify-between items-center p-5">
<div>
  <NuxtLink to="/" class="font-bold text-xl text-[#faa122]">ELECT-SHOP'S</NuxtLink> 
</div>

<div class="flex gap-5">
  <NuxtLink :active-class="'text-[#faa122]'" class="hover:text-[#faa122] hover:animate-pulse" to="/">Home</NuxtLink>
  <NuxtLink :active-class="'text-[#faa122]'" class="hover:text-[#faa122] hover:animate-pulse" to="/products">Products</NuxtLink>
  <NuxtLink :exact-active-class="'text-[#faa122]'" class="hover:text-[#faa122] hover:animate-pulse" to="/register">Register</NuxtLink>
  <UButton color="gray" icon="i-heroicons-shopping-cart" @click="isOpen = true">
      <h1>{{ cartStore.productTotal }}</h1>
      </UButton>

      <USlideover v-model="isOpen">
  <!-- <div class="p-4 flex-1">
   <Cart/>
  </div> -->
</USlideover>
</div>
  </div>
</nav>
  </div>
    </UContainer>
 
</template>

<script lang="ts" setup>
const isOpen = ref(false)
const cartStore = useCartStore()
</script>

<style>

</style>