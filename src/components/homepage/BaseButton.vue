<script>
export default {
  props: ['buttonDesc', 'buttonLink']
}
</script>

<template>
  <div class="text-center">
    <button :href="buttonDesc">
      {{ buttonDesc }}
    </button>
  </div>
</template>

<style scoped>
button {
  margin-top: 5rem;
  border-radius: 0%;
  border: 1px solid black;
  padding: 0.5rem 2rem;
  text-transform: uppercase;
  font-weight: 500;
}
</style>
