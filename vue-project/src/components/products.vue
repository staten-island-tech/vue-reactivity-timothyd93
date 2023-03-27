<script setup>
const products = [
  { name: "apple", price: 2.0, img: `C:\Users\timothy.deng\Documents\GitHub\vue-reactivity-timothyd93\vue-project\src\components\apple.jpg`},
  { name: "orange", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQh24pRhiUoM5TIn9K7S86c_uHhkjBUZuD9Jg&usqp=CAU" },
  { name: "pineapple", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ3jO9eMKEjXv0TQ1S736uUADRPnuu8mKyiVw&usqp=CAU" },
  { name: "grapes", price: 1.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8gU04X6jQNJ_BbTgvAGdoUYPEsg9ok8sS7w&usqp=CAU" },
  { name: "watermelon", price: 4.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAmbgB21P-h8gMIOtE3wXUjMaHRYfsfEJ-cA&usqp=CAU" },
  { name: "pear", price: 2.5, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTapfbRplXGkS0_olxze9Qs2ExfGlLdzYvGMQ&usqp=CAU" },
]
</script>

<template>
  <div class="home"  v-for="product in products">
    <img src={{product.img}}>
  <li> {{ product.name }}</li>
  </div>
</template>