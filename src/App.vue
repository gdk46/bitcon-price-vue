<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/digital-currency.png" height="200">
    <h1>Preços do Bitcoin</h1>
    <Bitcon
      :currencyBitcon="info"
    >
    </Bitcon>
  </div>
</template>

<script>
import Bitcon from './components/Bitcon.vue'

export default {
  name: 'App',
  
  components: {
    Bitcon
  }
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
