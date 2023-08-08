<template>
  <h3>Slots Fallback Content</h3>
  <p>A component without content provided can have fallback content in the slot tag.</p>
  <slot-comp>
    <!-- Empty -->
  </slot-comp>
  <slot-comp>
    <h4>This content is provided from App.vue</h4>
  </slot-comp>
</template>

<script></script>

<style>
  #app div {
    width: 150px;
  }
  h4 {
    text-align: center;
  }
</style>        
<script>
  export default {
    data() {
      return {
        foods: [
        { name: 'Apple', desc: 'Apples are a type of fruit that grow on trees.', url: 'img_apple.svg'},
        { name: 'Pizza', desc: 'Pizza has a bread base with tomato sauce, cheese, and toppings on top.', url: 'img_pizza.svg'},
        { name: 'Rice', desc: 'Rice is a type of grain that people like to eat.', url: 'img_rice.svg'},
        { name: 'Fish', desc: 'Fish is an animal that lives in water.', url: 'img_fish.svg'},
        { name: 'Cake', desc: 'Cake is something sweet that tates good but is not consodered healthy.', url: 'img_cake.svg'}
      ]
      }
    }
  }
</script>
<style>
  #wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  #wrapper > div {
    background-color: lightgreen;
  }
  footer > div {
    background-color: lightpink;
  }
  #wrapper img {
    display: block; 
    margin: 20% auto 0; 
    width: 60%;
  }
  h3, h4 {
    text-align: center;
  }
</style>      