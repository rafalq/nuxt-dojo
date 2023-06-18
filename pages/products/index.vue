<script setup>
    useHead({
        title: 'Products'
    })

    definePageMeta({
        layout: 'products'
    })

    const {data: products} = await useFetch('https://fakestoreapi.com/products')
</script>

<template>
    <h1 class="mb-2 text-2xl">PRODUCTS</h1>
    <div class="grid grid-cols-4 gap-5">
        <div v-for="p in products">
            <ProductCard :product="p" />
        </div>
    </div>
</template>