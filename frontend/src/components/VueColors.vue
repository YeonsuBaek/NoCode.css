<template>
  <div class="colors">
    <header class="sub-header">
      <h2 class="sub-title">Colors</h2>
      <button class="creating-button" type="button">create</button>
    </header>

    <ul class="color-list">
      <li class="color-item">
        <button class="color-copy-button" type="button"></button>
        <pre class="color-name" contenteditable="true" spellcheck="false">
#3B5998</pre
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.colors {
  margin-top: calc(48px + 60px);
}

.color-list {
  display: flex;
  align-items: start;
  justify-content: start;
  flex-wrap: wrap;
}

.color-item {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  margin: 0 16px 16px 0;
}

.color-item:nth-child(4n) {
  margin-right: 0;
}

.color-copy-button {
  position: relative;
  margin-bottom: 4px;
  width: 160px;
  height: 160px;
  background: #3b5998;
  border-radius: 8px;
}

.color-copy-button:is(:hover, :active)::before {
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.2);
  border-radius: 8px;
}

.copy-icon {
  width: 36px;
  height: 36px;
  overflow: hidden;
}

.copy-icon img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.color-copy-button:hover::before {
  content: "Copy";
}

.color-copy-button:active::before {
  content: "Copied!";
}

.color-copy-button:is(:hover, :active)::before {
  color: #fff;
  font-size: 18px;
  font-weight: 700;
}

.color-name {
  margin-left: 4px;
  font-size: 18px;
  font-weight: 400;
  outline: none;
}
</style>
