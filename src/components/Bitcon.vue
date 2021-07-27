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
import axios from 'axios'


export default {
  name: "Bitcon",
  props: ['currencyBitcon'],

  data() {
    return {
      info: null,
    }
  },

  mounted() {
    axios
      .get('https://api.coindesk.com/v1/bpi/currentprice.json')
      .then((response) => {
        this.info = response.data.bpi;
        return this.info;
      })
  },
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
