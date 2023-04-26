<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <nuxt-link to="/" class="font-bold">Nuxt Dojo</nuxt-link>
                <ul class="flex gap-4">
                    <li>
                        <nuxt-link to="/">Home</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/about">About</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/products" class="btn">Products</nuxt-link>
                    </li>
                </ul>
            </nav>
        </header>

        <!-- output page content -->
        <div class="container mx-auto">
            <slot />
        </div>
    </div>
</template>

<style >
h2{
        margin-bottom: 20px;
        font-size: 36px;
    }
    p{
        margin: 20px 0;
    }
.router-link-exact-active{
    color: #12b488;
}
</style>