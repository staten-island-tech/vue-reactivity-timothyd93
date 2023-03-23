<template>
    <div class="home">
    <li v-for="product in products"> {{ product.name }}</li>
    </div>
</template>

<script>
const products = ref([
  { name: apple, price: 2.0 },
  { name: orange, price: 3.0 },
  { name: pineapple, price: 3.0 },
  { name: grape, price: 1.0 },
  { name: watermelon, price: 4.0 },
  { name: pear, price: 2.5 },
])
</script>

