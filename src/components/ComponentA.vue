<script setup lang="ts">
const props = defineProps(["description"]);
const {description} = props;

</script>

<template>
    <h3>
      Hello {{description}} - From A
    </h3>
</template>

<style scoped>

h3 {
  color: darkgreen;
  padding: 1em;
}
</style>
