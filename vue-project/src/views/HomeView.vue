<template>
  <main>
    <h1 id="header">Fruit Store Online Shopping Cart</h1>
    <h2 id="total">Total: ${{ total }}</h2>
    <div id="container">
    <div v-for="fruit in fruits">
        <Card
      :key ="fruit.name"
      :name ="fruit.name"
      :price ="fruit.price"
      :img = "fruit.img"
      />
      <button id="button" v-on:click="addPrice(fruit.price)"> Add to Cart</button>
    </div>
    <!-- <div v-for="fruit in fruits">
      <List  
      :key="fruit.name"
      :name ="fruit.name"
      />
    </div> -->
  </div>  
  </main>
</template>

<script>
import Card from "../components/products.vue"
import List from "../components/shoppinglist.vue"
export default {
  name: "array",
  components: {
    Card,
    List,
  },
  data() {
    return {
      fruits: [
      { name: "Apple", price: 2.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTn4jedgV_XfyLOBuegpPVJQRtwFViVI7dDWw&usqp=CAU"},
    { name: "Orange", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYsNDHoyYYbfJPLaz9lRPuMEoMQUsR3JdN2A&usqp=CAU" },
    { name: "Pineapple", price: 3.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ3jO9eMKEjXv0TQ1S736uUADRPnuu8mKyiVw&usqp=CAU" },
    { name: "Grapes", price: 1.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8gU04X6jQNJ_BbTgvAGdoUYPEsg9ok8sS7w&usqp=CAU" },
    { name: "Watermelon", price: 4.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAmbgB21P-h8gMIOtE3wXUjMaHRYfsfEJ-cA&usqp=CAU" },
    { name: "Pear", price: 2.0, img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTapfbRplXGkS0_olxze9Qs2ExfGlLdzYvGMQ&usqp=CAU" },
      ],
      total: 0
    };
  },
  methods: {
    addPrice(fruits) {
    this.total += fruits
    console.log(this.total)
    },
    shoppingList(){
    
    },
  },
};
</script>

<style>
#total {
  text-align: center;
}

#header{
  text-align: center;
  margin-bottom: 4rem;
}

#button{
  margin-left: ;
}

#container{ 
display: flex;
flex-wrap: wrap;
justify-content: space-evenly;
text-align: center;
}
.cards {
  text-align: center;
  height: 500px;
  width: 500px;
  margin-top: 1rem;
}
.img{
  width: 300px;
  height: 300px;
}

#body{
  background-color: #FAF9F6;
}
</style>
