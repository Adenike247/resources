<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode']
}
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #ff00ff;
  border: 1px solid #ff00ff;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #ff00bf;
  border-color: #ff00bf;
}

.flat {
  background-color: transparent;
  color: #777;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #edd2ff;
}
</style>