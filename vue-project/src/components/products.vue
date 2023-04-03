<template>
    <div class="cards">
      <img :src="img" class="img" />
      <p>{{ name }}</p>
      <p> ${{ price }}.00</p>
    </div>
  </template>
  

<script>
export default {
  name: "Card",
  props: {
    name: String,
    price: Number,
    img: String,
  },
}
</script>
