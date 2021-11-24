<template>
    <div id="app">
        <!-- HEADER -->
        <header>
            <Header />
            <Jumbotron img="jumbotron.jpg" />
        </header>

        <!-- MAIN -->
        <main>
            <Content />
            <Shops />
        </main>

        <!-- FOOTER -->
        <footer>
            <FooterLinks />
            <Social />
        </footer>
    </div>
</template>

<script>
/* Import Components */
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Content from "./components/Content.vue";
import Shops from "./components/Shops.vue";
import FooterLinks from "./components/FooterLinks.vue";
import Social from "./components/Social.vue";

/* Import Data */
import data from './data/dc-comics';

export default {
    name: "App",
    components: {
        Header,
        Jumbotron,
        Content,
        Shops,
        FooterLinks,
        Social,
    },
    data() {
        return {
            data,
        };
    },
};
</script>

<style lang="scss">
@import "./styles/general";

#app {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

main {
    flex-grow: 1;
}
</style>
