<template>
    <div class="container">
        <img src="../assets/dc-logo.png" alt="DC Logo">
        <ul>
            <li v-for="(link, index) in navLinks" :class="{active: link.isActive}" :key="`headerNavLink-${index}`">
                <a :href="link.url">{{ link.text }}</a>
            </li>
        </ul>
    </div>  
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            navLinks: [
                {
                    text: 'Characters',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Comics',
                    url: '/',
                    isActive: true,
                },
                {
                    text: 'Movies',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'TV',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Games',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Collectibles',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Videos',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Fans',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'News',
                    url: '/',
                    isActive: false,
                },
                {
                    text: 'Shop',
                    url: '/',
                    isActive: false,
                },
            ],
        }
    }
}
</script>

<style scoped lang="scss">
.container {
    display: flex;

    img {
        padding: 20px 0;
    }
}

ul {
    list-style: none;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    flex-grow: 1;

    li {
        display: flex;
        align-items: center;
        margin: 0 10px;
        height: 100%;

        &:last-child {
            margin: 0;
        }

        &.active {
            color: blue;
            border-bottom: 4px solid blue;
        }

        a {
            text-decoration: none;
            text-transform: uppercase;
        }
    }

}
</style>