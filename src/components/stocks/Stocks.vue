<template>
  <div>
    <h1>Stocks Template</h1>
    <div class="row">
      <div v-for="stock in stocks" :key="stock.id">
        <Stock :stock="stock"></Stock>
      </div>
    </div>
  </div>
</template>
<script>
import {mapGetters} from 'vuex';
import Stock from './Stock.vue';
export default {
  computed:{
    ...mapGetters([
      'stocks',
    ])
  },
  components: {
    Stock
  },
}
</script>