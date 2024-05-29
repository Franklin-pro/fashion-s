<template>
  <div>
    <div v-for="item in pro.length" :key="item.id">
      {{ item.name }}
    </div>

 

   
<div class="py-5 flex justify-around items-center">
  <h2>TOTAL Price : {{ cartStore.total }}</h2>
  <Modal/>
</div>
    
  </div>
</template>

<script setup>
import { useCartStore } from '~/stores/carts';
import products from '~/data';
const pro = ref(products)
const cartStore = useCartStore()
</script>

<style>

</style>