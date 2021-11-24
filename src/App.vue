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
};
</script>

<style lang="scss">
@import "./styles/general";
@import "./styles/vars";

#app {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

main {
    flex-grow: 1;
}
</style>
