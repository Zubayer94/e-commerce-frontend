<template>
  <div>
    <AppHeader />
    <BuyNavBar />
    <BuySlider />
    
    <nuxt/>

    <AppFooter />
  </div>
</template>

<script>
import AppHeader from '../components/home/AppHeader.vue'
import AppFooter from '../components/home/AppFooter.vue'
import BuyNavBar from '../components/buy/BuyNavBar.vue'
import BuySlider from '../components/buy/BuySlider.vue'
export default {
  components: { AppHeader, AppFooter, BuyNavBar, BuySlider },

}
</script>

<style>

</style>
