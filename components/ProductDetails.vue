<script setup>
   const {product} = defineProps(['product']) 
</script>

<template>
  <div class="card">
    <div class="grid grid-cols-2 gap-10">
        <div class="p-7">
            <img :src="product.image" alt="product image" class="mx-auto my-7">
        </div>
        <div class="p-7">
            <h2 class="text-4xl my-7">{{ product.title }}</h2>
            <p class="text-xl my-7">Price: ${{ product.price }}</p>
            <h3 class="pb-2 mb-4 font-bold border-b-2">Product Description</h3>
            <p class="mb-7">{{ product.description }}</p>
            <div class="flex justify-end">
                <button class="flex items-center btn">
                    <i class="mr-2 material-icons">add_shopping_cart</i>
                    <span>ADD TO CART</span>
                </button>
            </div>
        </div>
    </div>
  </div>
</template>

<style scoped>
    img {
        max-width: 400px;
    }
</style>