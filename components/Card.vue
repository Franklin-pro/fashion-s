<template>
  <UContainer as="section">
    <div class="grid  grid-cols-3 py-5">
    <div v-for="item in products" :key="item.id">
      <div class="p-4">
        <UCard>
 <div>
  <img :src="item.image" alt="">
  <h1>{{ item.name }}</h1>
  <p>{{ item.description }}</p>
  <div class="flex justify-between items-center py-3">
    <b>{{ item.price }} RWF</b>
  <UIcon name="i-heroicons-shopping-cart"  class="text-xl cursor-pointer hover:text-[#faa122]" @click="cartStore.add"/>
  </div>

 </div>
  </UCard>
      </div>

    </div>
  </div>
  </UContainer>

</template>

<script lang="ts" setup>
import products from '~/data';

const cartStore = useCartStore()
</script>

<style>

</style>