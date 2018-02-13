<template>
  <div class="col-md">
    <div class="card">
      <div class="card-header">
        {{stock.name}}
      </div>
      <div class="card-body">
        <h5 class="card-title">{{stock.name}} <small>(Price: ${{stock.price}})</small></h5>
        <p class="card-text">
          <input type="number" class="form-control" placeholder="Quantity" v-model="quantity">
        </p>
        <button type="button" class="btn btn-primary" :disabled="quantity <= 0 || Number.isInteger(quantity)" @click="buyStock">Buy</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["stock"],
  data() {
    return {
      quantity: 0,
    }
  },
  methods: {
    buyStock() {
      const order = {
        stockId: this.stock.id,
        stockPrice: this.stock.price,
        quantity: this.quantity,
      };
      console.log(order);
      this.$store.dispatch('buyStock', order);
      this.quantity = 0;
    }
  }
}
</script>
