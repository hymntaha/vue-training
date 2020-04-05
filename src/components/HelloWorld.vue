<template>
  <div>
    <p v-if="show">You can see me!</p>
    <p v-else>Now you see me!</p>
    <template v-if="show">
      <h2>Heading</h2>
      <p>Inside a template</p>
    </template>
    <p v-show="show">Do you see me!</p>
    <button @click="show =!show">Switch</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: function() {
    return {
      show: true
    };
  },
  props: {
    msg: String
  }
};
</script>

<style scoped></style>
