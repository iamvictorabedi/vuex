<template>
  <div id="product-list-one">
<h1>Product List One</h1>
<ul>
  <li v-for="product in products">
    <span class='name'>{{product.name}}</span>
        <span class='amount'>${{product.price}}</span>

  </li>
</ul>
  </div>
</template>

<script>
export default {
  props: ['products'],
  data () {
  return {

  }
  }
}
</script>

<style scoped>
#product-list-one{
    background: #FFF8B1;
    box-shadow: 1px 2px 3px rgba(0,0,0,0.2);
    margin-bottom: 30px;
    padding: 10px 20px;
}
#product-list-one ul{
    padding: 0;
}
#product-list-one li{
    display: inline-block;
    margin-right: 10px;
    margin-top: 10px;
    padding: 20px;
    background: rgba(255,255,255,0.7);
}
.amount{
    font-weight: bold;
    color: #E8800C;
}

</style>
