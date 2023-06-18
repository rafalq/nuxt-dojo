<script setup>
    const {product} = defineProps(['product'])
</script>

<template>
    <div class="text-center card">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="m-4 font-bold text-gray-500 truncate">{{ product.title }}</p>
        <NuxtLink :to="`/products/${product.id}`"><p class="my-4 btn">VIEW DETAILS</p></NuxtLink>
    </div>
</template>