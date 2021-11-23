<template>
  <div id="app">
    <!-- HEADER -->
    <header>
      <Header />
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
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import Shops from './components/Shops.vue'
import FooterLinks from './components/FooterLinks.vue'
import Social from './components/Social.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Shops,
    FooterLinks,
    Social
  }
}
</script>

<style lang="scss">
@import './styles/general';

#app {
  display: flex;
  flex-direction: column;
}

main {
  flex-grow: 1;
}
</style>
