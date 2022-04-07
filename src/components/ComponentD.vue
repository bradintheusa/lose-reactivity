<script setup lang="ts">

const props = defineProps(["description"]);
const description = props.description;

</script>

<template>
    <h3>
      Hello {{description}} - From D
    </h3>
</template>

<style scoped>

h3 {
  color: darkcyan;
  padding: 1em;
}
</style>
