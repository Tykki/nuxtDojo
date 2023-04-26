<template>
    <div>
        <section class="grid grid-cols-4 gap-5">
            <div v-for="p in products" :key="p.id">
                <ProductCard :product="p" />
            </div>
        </section>
    </div>
</template>

<script setup lang="ts">
definePageMeta({
    layout: 'products'
})

// fetch products
const {data: products} = await useFetch('https://fakestoreapi.com/products')

useHead({
    title: 'Nuxt Dojo | Merch',
    meta: [
        {
            name: 'description', content: 'Nuxt 3 Merch'
        }
    ]
})
</script>

<style scoped>

</style>