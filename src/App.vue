<template>
  <div>
    <h2>{{title}}</h2>


   <hr>
    <section-one :product = "product"></section-one>
    <hr>
    <section-two :product = "product"></section-two>
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
      title: 'Test Javascript Spread',
      product: {id: 12, price: 29.5}
    }
  },

  mounted() {
    this.product.num = 1
  },

  methods: {
    
  }
}
</script>

<style>

</style>
