<template>
  <div>
    <AppSlider />
    <Content />
  </div>
</template>

<script>
import AppSlider from '../components/home/AppSlider.vue'
import Content from '../components/home/Content.vue'
export default {
  components: { Content, AppSlider },
  name: 'IndexPage'
}
</script>
