<script setup lang="ts">
import {toRef} from "vue";

const props = defineProps(["description"]);
const description = toRef(props.description,"desc");

</script>

<template>
  <h2>Component C</h2>

  <p>This is not reactive</p>
  <pre>
  const description = toRef(props.description,"desc");

</pre>
  <h3>
    {{description}}
  </h3>
</template>

<style scoped>

h3 {
  color: darkred;
  padding: 1em;
}
</style>
