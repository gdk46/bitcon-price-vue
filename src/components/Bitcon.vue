<template>
  <div class="currency">
    <div
      v-for="currency in info"
      class="currency"
      :key="currency.description"
      >
      {{ currency.description }}:
      <span class="lighten">
        <span v-html="currency.symbol"></span> 
        {{ currency.rate_float | currencydecimal }}
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bitcon",
  props: {
    currencyBitcon: Object
  },

  data() {
    return {
      info: this.currencyBitcon,
    }
  },

  methods: {},

  filters: {
    currencydecimal(value) {
      return value.toFixed(2)
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.currency {
  width: 20rem;
  background-color: #ececec;
  padding: .75rem ;
  margin-left: auto;
  margin-right: auto;
  border-radius: .5rem;
}

</style>
