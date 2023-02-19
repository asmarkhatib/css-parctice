<template>
  <HelloWorld />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-weight: 400;
  line-height: 1.5385;
  font-family: "Poppins", sans-serif;
  color: #333;
  text-align: left;
  font-size: 14px;
  letter-spacing: normal;
}
</style>
