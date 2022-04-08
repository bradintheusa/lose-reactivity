<script setup lang="ts">
import {computed} from "vue";
const props = defineProps(["description"]);

const description = computed(() => props.description.toLowerCase())

</script>

<template>
  <h2>Component D</h2>

  <p>This is reactive</p>
  <pre>
  const description = computed(() => props.description.toLowerCase())

</pre>
  <h3>
    {{description}}
  </h3>
</template>

<style scoped>

h3 {
  color: darkgoldenrod;
  padding: 1em;
}
</style>
