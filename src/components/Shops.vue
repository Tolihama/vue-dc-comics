<template>
    <div>
        <div class="container">
            <ul>
                <li v-for="(shop, index) in shopList" :key="`shop-${index}`">
                    <!-- <img :src="`../assets/buy-comics-digital-comics.png`" :alt="shop.text"> -->
                    <img src="../assets/buy-comics-digital-comics.png" :alt="shop.text">
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
                {
                    text: 'DC Merchandise',
                    logoImg: 'buy-comics-merchandise.png',
                    url: '/',
                },
                {
                    text: 'Subscription',
                    logoImg: 'buy-comics-subscriptions.png',
                    url: '/',
                },
                {
                    text: 'Comic Shop Locator',
                    logoImg: 'buy-comics-shop-locator.png',
                    url: '/',
                },
                {
                    text: 'DC Power Visa',
                    logoImg: 'buy-dc-power-visa.svg',
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
    display: flex;
    justify-content: center;
    align-items: center;

    .container {
        padding: 50px 0;

        ul {
            display: flex;
            list-style: none;

            li {
                display: flex;
                justify-content: center;
                align-items: center;

                img {
                    height: 50%;
                    margin-right: 10px;
                }

                a {
                    color: #fff;
                    text-transform: uppercase;
                    text-decoration: none;
                }
            }
        }

    }
}
</style>