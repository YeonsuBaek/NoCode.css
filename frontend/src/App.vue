<template>
  <div>
    <VueHeader />
    <VueContent />
  </div>
</template>

<script>
import VueHeader from "./components/VueHeader.vue";
import VueContent from "./components/VueContent.vue";

export default {
  components: {
    VueHeader,
    VueContent,
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
  max-width: 688px;
}

.sub-header {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  padding: 0 10px;
  margin-bottom: 16px;
  width: 100%;
}

.sub-title {
  color: #2d2e2f;
  font-size: 24px;
  font-weight: 400;
}

.creating-button {
  color: #0085f9;
  font-size: 18px;
  font-weight: 700;
}

.creating-button:is(:hover, :active) {
  color: #0072d6;
}
</style>
