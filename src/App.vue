<template>
  <div id="app">
    <Heading />
    <Banners />
    <Benefits />
    <Brands />
    <Products />
    <Institutional />
    <Footer />
  </div>
</template>

<script lang="ts">

import { Component, Vue } from 'vue-property-decorator';
import Heading from './components/Heading.vue';
import Banners from './components/Banners.vue';
import Benefits from './components/Benefits.vue';
import Brands from './components/Brands.vue';
import Products from './components/Products.vue';
import Institutional from './components/Institutional.vue'
import Footer from './components/Footer.vue';

@Component({
  components: {
    Heading,
    Banners,
    Benefits,
    Brands,
    Products,
    Institutional,
    Footer
  },
})
export default class App extends Vue {


}
</script>

<style src="./assets/styles/main.scss" lang="scss">

</style>
