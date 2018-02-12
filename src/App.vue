<template>
  <div class="container">
    <app-header></app-header>
    <router-view></router-view>
  </div>
</template>

<script>
import Header from './components/Header.vue'
export default {
  components: {
    'app-header': Header
  },
  data: {
    
  }
}
</script>
<style lang="css" scoped>

</style>
