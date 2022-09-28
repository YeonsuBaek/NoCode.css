<template>
  <header class="global-header">
    <h1 class="title">NoCode.css</h1>
    <button class="sharing-button" type="button">Sharing</button>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
.global-header {
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 40px;
  width: 100%;
  height: 60px;
  background-color: #fff;
  border-bottom: 1px solid #d7dde3;
}
.title {
  color: #2d2e2f;
  font-size: 24px;
  font-weight: 700;
}

.sharing-button {
  padding: 8px 12px;
  color: #fff;
  background-color: #0085f9;
  border-radius: 4px;
}

.sharing-button:is(:hover, :active) {
  background-color: #0072d6;
}
</style>
