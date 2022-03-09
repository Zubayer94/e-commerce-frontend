<template>
  <div>
    <AppHeader/>
    <AppNavBar />

    <nuxt/>

    <AppFooter />
  </div>
</template>

<script>
import AppFooter from '../components/home/AppFooter.vue'
import AppHeader from '../components/home/AppHeader.vue'
import AppNavBar from '../components/home/AppNavBar.vue'
export default {
  components: { AppHeader, AppNavBar, AppFooter },

}
</script>

<style>

</style>
