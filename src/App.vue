<template>
  <div id="app">
<product-list-one v-bind:products='products'></product-list-one>
<product-list-two v-bind:products='products'></product-list-two>
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne.vue'
import ProductListTwo from './components/ProductListTwo.vue'

export default {
  components: {
    'product-list-one': ProductListOne,
    'product-list-two': ProductListTwo
  },
  name: 'app',
  data () {
  return {
    products: [
      {name: 'Vaseline', price: 20},
            {name: 'Pints', price: 20},
                  {name: 'Eggs', price: 30},
                        {name: 'Olsns', price: 30}
    ]

  }
  }
}
</script>

<style>
body{
  font-family: 'Ubuntu';
  color: #555;
}
</style>
