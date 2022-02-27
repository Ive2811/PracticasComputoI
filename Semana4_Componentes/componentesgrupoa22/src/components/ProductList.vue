<template>
<div id="root">
<h2>Products</h2>

<div class="row">
  <div class="col-sm-6" v-for="(item,index) in items" v-bind:key="index">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">{{item.productName}}</h5>
        <p class="card-text">{{item.description}}</p>
        <p>$ {{item.price}}</p>
        <input type="number" v-model="item.quantity">
        <a href="#" class="btn btn-primary" @click="addProduct(index)">Add cart</a>
      </div>
    </div>
  </div>
  
</div>
</div>
</template>
<script>
import products from '../data/products.json'

export default{
    name:'ProductList',

    data(){
        return{
            items:products,
            cartProducts:[],
            itemCount:0
        }
     },
  }
</script>