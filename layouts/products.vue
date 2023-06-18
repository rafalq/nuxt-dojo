<script setup></script>

<template>
    <TheHeader />
    <small class="mt-2 ml-2">-- products layout --</small>
    <div class="container p-4 mx-auto"><slot /></div>
</template>

<style scoped>
    .router-link-exact-active {
        color: whitesmoke;
    }
</style>