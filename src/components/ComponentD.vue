<script setup lang="ts">

const props = defineProps(["description"]);
const description = props.description;

</script>

<template>
  <h2>Component D</h2>

  <p>This is not reactive</p>
  <pre>
  const description = props.description;

</pre>
  <h3>
    {{description}}
  </h3>
</template>

<style scoped>

h3 {
  color: darkcyan;
  padding: 1em;
}
</style>
