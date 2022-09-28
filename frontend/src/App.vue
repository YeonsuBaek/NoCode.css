<template>
  <div>
    <VueHeader />
  </div>
</template>

<script>
import VueHeader from "./components/VueHeader.vue";

export default {
  components: {
    VueHeader,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}

body {
  font-family: "Roboto", sans-serif;
  color: #3c3d3f;
}

button {
  border: 0;
  outline: 0;
  cursor: pointer;
  background-color: transparent;
}

li {
  list-style-type: none;
}

.container {
  width: 100%;
  padding: 0;
  margin: 0 auto;
  max-width: 704px;
  background: pink;
}
</style>
