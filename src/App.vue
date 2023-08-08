<template>
  <h1>Food</h1>
  <p>Components created with v-for based on an array.</p>
  <div id="wrapper">
    <food-item
      v-for="x in foods"
      v-bind:food-name="x"/>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        foods: ['Apples','Pizza','Rice','Fish','Cake']
      };
    }
  }
</script>