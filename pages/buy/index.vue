<template>
  <div>
    <BuySlider />
    <BuyHomeContent />
  </div>
</template>

<script>
import BuyHomeContent from '../../components/buy/BuyHomeContent.vue'
import Content from '../../components/home/Content.vue'
export default {
  components: { Content, BuyHomeContent },
  layout: 'buy',

}
</script>

<style>

</style>
