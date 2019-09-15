<template>
  <div>
    <h2>{{title}}</h2>
    <button @click="fetchCurrencyData">Fetch Currencty Data</button>
    <section-one></section-one>
    <hr>
    <section-two></section-two>
  </div>
</template>

<script>

import SectionOne from './components/SectionOne'
import SectionTwo from './components/SectionTwo'
export default {
  components: {
    SectionOne,
    SectionTwo
  },
  data() {
    return {
      title: 'Test Javascript Spread'
    }
  },

  mounted() {
    console.log('oops')
  },

  methods: {
    fetchCurrencyData() {
      fetch('https://api.exchangeratesapi.io/latest?base=AUD&symbols=CNY')
      .then((response)=> {return response.json()})
      .then((data)=>{console.log(data)})
    }
  }
}
</script>

<style>

</style>
