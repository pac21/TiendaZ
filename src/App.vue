<template>
  <div id="app">
    <div id="nav">
      <template v-if="path">
        <Navegation/>
      </template>
      <template v-else>
        <NavegationA/>
      </template>
      <template>
        <Footer/>
      </template>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Navegation from '@/components/Layout/Client/Navigation.vue'
import NavegationA from '@/components/Layout/Administration/Navigation.vue'
import Footer from '@/components/Footer/Footer.vue'
export default {
  name: 'App',

  components: {
    Navegation,
    NavegationA,
    Footer
  },
  data() {
      return {
        path: '/'
      }
    },
};
</script>

<style lang="scss">
  @import './scss/App.scss';
</style>