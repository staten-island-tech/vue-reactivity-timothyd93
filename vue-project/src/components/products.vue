<script setup>
const products = [
  { name: "apple", price: 2.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTn4jedgV_XfyLOBuegpPVJQRtwFViVI7dDWw&usqp=CAU"},
  { name: "orange", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYsNDHoyYYbfJPLaz9lRPuMEoMQUsR3JdN2A&usqp=CAU" },
  { name: "pineapple", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ3jO9eMKEjXv0TQ1S736uUADRPnuu8mKyiVw&usqp=CAU" },
  { name: "grapes", price: 1.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8gU04X6jQNJ_BbTgvAGdoUYPEsg9ok8sS7w&usqp=CAU" },
  { name: "watermelon", price: 4.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAmbgB21P-h8gMIOtE3wXUjMaHRYfsfEJ-cA&usqp=CAU" },
  { name: "pear", price: 2.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTapfbRplXGkS0_olxze9Qs2ExfGlLdzYvGMQ&usqp=CAU" },
]
</script>
<template>
    <div id="app">
    <div v-for="product in products" class="cards">
      <img :src="product.img" class="img" />
      <p>{{ product.name }}</p>
      <button>${{ product.price }}.00</button>
    </div>
  </div>
  </template>
  
  <style>
  #app{ 
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
  }
  .cards {
    text-align: center;
    height: 500px;
    width: 500px;
  }
  .img{
    width: 300px;
    height: 300px;
  }
  </style>