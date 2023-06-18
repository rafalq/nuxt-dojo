<script setup>
    // const {data} = await useFetch('/api/ninja?name=rafalq', {
    //     method: 'POST',
    //     body: {age: 43}
    // })

    // const {data} = await useFetch('/api/ninja')

const {data} = await useFetch('/api/currency/GBP')
</script>

<template>
    <h1 class="mb-2 text-2xl">ABOUT</h1>
    <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem, distinctio beatae. Minus error voluptas neque rerum earum officiis provident cum!</p>
    <pre>{{ data }}</pre>
</template>