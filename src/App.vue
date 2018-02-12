<template>
  <div class="container">
    <appHeader></appHeader>
    <router-view></router-view>
    <input type="text" ref="input">
  </div>
</template>

<script>
import Header from './components/Header.vue'
export default {
  components: {
    appHeader: Header
  },
  data: {
    
  }
}
</script>
<style lang="css" scoped>

</style>
