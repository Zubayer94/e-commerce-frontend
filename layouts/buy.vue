<template>
  <div>
    <AppHeader />

    <nuxt/>

    <AppFooter />
  </div>
</template>

<script>
import AppHeader from '../components/home/AppHeader.vue'
import AppFooter from '../components/home/AppFooter.vue'
export default {
  components: { AppHeader, AppFooter },

}
</script>

<style>

</style>
