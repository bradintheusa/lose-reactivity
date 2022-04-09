<script setup lang="ts">
import {toRefs} from "vue";
const props = defineProps(["description"]);

const {description} = toRefs(props);
const d  = description;
</script>

<template>
  <h2>Component B</h2>
  <p>This works</p>

  <p>As you can see it is reactive</p>
  <pre>
  const {description} = toRefs(props);
</pre>
  <h3>
    {{description}}
  </h3>
</template>

<style scoped>

h3 {
  color: navy;
  padding: 1em;
}
</style>
