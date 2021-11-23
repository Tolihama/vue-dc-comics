<template>
    <div>
        <div class="container">
            <ul>
                <li v-for="(shop, index) in shopList" :key="`shop-${index}`">
                    <img :src="`@/assets/${shop.logoImg}`" :alt="shop.text">
                    <a :href="shop.url"> {{ shop.text }} </a>
                </li>
            </ul>

        </div>
    </div>
</template>

<script>
export default {
    name: 'Shops',
    data() {
        return {
            shopList: [
                {
                    text: 'Digital Comics',
                    logoImg: 'buy-comics-digital-comics.png',
                    url: '/',
                },
            ],
        };
    },
}
</script>

<style scoped lang="scss">
div {
    background: #0282f9;
    padding: 50px 0;
}
</style>