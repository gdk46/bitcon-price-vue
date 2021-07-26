<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/digital-currency.png" height="200">
    <h1>Preços do Bitcoin</h1>
    <Bitcon
      v-bind:currencyBitcon="info"
    >
    </Bitcon>
  </div>
</template>

<script>
import Bitcon from './components/Bitcon.vue'
import axios from 'axios'

export default {
  name: 'App',
  
  components: {
    Bitcon
  },

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
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
