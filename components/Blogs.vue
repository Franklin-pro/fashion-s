<template>
  <div>
    <h1 class="p-5 text-center text-3xl">OUR BLOGS</h1>
    <UContainer>
      <div class="grid grid-cols-2 gap-5">
 
 <div v-for="item in items" :key="item.id" class="hover:scale-105 hover:shadow-lg shadow-md duration-300 hover:border-green-500 hover:border-lg">
<UCard>
  <div  class="flex gap-5 items-center">
    <div class="w-[600px] ">
    <img :src="item.image" alt="" class="w-full h-[200px] cover">
  </div>
  <div>
    <h1 class="py-2 font-semibold">{{ item.heading }}</h1>
<p>{{ item.description }}</p>
<NuxtLink to="/" class="text-blue-400">READ MORE...</NuxtLink>
<p class="text-gray-400 p-2">23/dec/2024</p>
  </div>

  </div>
 
  

</UCard>

</div>
</div>
    </UContainer>
 


  </div>

</template>

<script setup>




const items = [
  {
    heading:'Ishimwe Christian',
    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus cum earum velit, vero minima dolorum? Rem quisquam totam repudiandae.',
    icon : 'i-heroicons-heart',
    image:"https://images.pexels.com/photos/977841/pexels-photo-977841.jpeg?auto=compress&cs=tinysrgb&w=800",
    discount :'price:800$',
    price : 'price: 500$',
    icons:'i-heroicons-shopping-cart',
    sold:'1000 sold'


  },
  {
  
    heading:'Ishimwe Chance',
    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus cum earum velit, vero minima dolorum? Rem quisquam totam repudiandae.',
    icon : 'i-heroicons-heart',
   


  },
  {
    heading:'Gisubizo julien',
    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus cum earum velit, vero minima dolorum? Rem quisquam totam repudiandae.',
    icon : 'i-heroicons-heart',
    discount :'price:800$',
    price : 'price: 500$',
    icons:'i-heroicons-shopping-cart',
    sold:'1000 sold'


  },
  {
    heading:'Young Mill',
    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus cum earum velit, vero minima dolorum? Rem quisquam totam repudiandae.',
    icon : 'i-heroicons-heart',
    discount :'price:800$',
    price : 'price: 500$',
    icons:'i-heroicons-shopping-cart',
    sold:'1000 sold'


  },
  
  {
    heading:'Justin King',
    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos natus cum earum velit, vero minima dolorum? Rem quisquam totam repudiandae.',
    icon : 'i-heroicons-heart',
    discount :'price:800$',
    price : 'price: 500$',
    icons:'i-heroicons-shopping-cart',
    sold:'1000 sold'


  },
  

 
]
</script>

<style>

</style>