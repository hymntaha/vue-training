<template>
  <div>
    <p v-if="show">You can see me!</p>
    <p>Do you also see me</p>
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
