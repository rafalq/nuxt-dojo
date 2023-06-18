<script setup></script>

<template>
    <header class="bg-white shadow-sm">
        <nav class="container flex justify-between p-4 mx-auto">
            <NuxtLink to="/" class="font-bold">Nuxt Dojo</NuxtLink>
            <ul class="flex gap-4">
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
    ul {
        list-style: none;
    }
    .router-link-exact-active {
        color: #12b488;
    }
    .btn.router-link-exact-active {
        background-color: whitesmoke;
    }
</style>
