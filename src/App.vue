<template>
    <Home/>
</template>

<script>
import Home from "./components/Home.vue";

export default {
  components: {
    Home    
  }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}

body {
  background: #070A1B;
}

screen {
  height: 100vh;
  width: 100vw;
}

input[type="email"],
input[type="password"] {
  background: transparent;
  outline: none;
  border: none;
  border-bottom: 0.5px solid #8D8484;
  color: #fff;
  padding: .5em;
}

input[type="submit"] {
  cursor: pointer;
}

</style>