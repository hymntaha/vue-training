<template>
  <div>
    <!--    <p v-if="show">You can see me!</p>-->
    <!--    <p v-else>Now you see me!</p>-->
    <!--    <template v-if="show">-->
    <!--      <h2>Heading</h2>-->
    <!--      <p>Inside a template</p>-->
    <!--    </template>-->
    <!--    <p v-show="show">Do you see me!</p>-->
    <!--    <button @click="show =!show">Switch</button>-->
    <ul>
      <li v-for="(ingredient, i) in ingredients" :key="ingredient">
        {{ ingredient }} ({{ i }})
      </li>
    </ul>
    <hr />
    <ul>
      <li v-for="person in persons" :key="person">
        <span v-for="value in person" :key="value"> {{value}} </span>
      </li>
    </ul>
    <!--    <template v-for="(ingredient, index) in ingredients">-->
    <!--      <h1>{{ingredient}}</h1>-->
    <!--      <p>{{index}}</p>-->
    <!--    </template>-->
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: function() {
    return {
      // show: true
      ingredients: ["meat", "fruit", "cookies"],
      persons: [
        { name: "Max", age: 27, color: "red" },
        { name: "Anna", age: "unknown", color: "blue" }
      ]
    };
  },
  props: {
    msg: String
  }
};
</script>

<style scoped></style>
