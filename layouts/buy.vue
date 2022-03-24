<template>
  <div>
    <AppHeader />
    <BuyNavBar />

    <nuxt/>

    <AppFooter />
  </div>
</template>

<script>
import AppHeader from '../components/home/AppHeader.vue'
import AppFooter from '../components/home/AppFooter.vue'
import BuyNavBar from '../components/buy/BuyNavBar.vue'
export default {
  components: { AppHeader, AppFooter, BuyNavBar },

}
</script>

<style>

</style>
