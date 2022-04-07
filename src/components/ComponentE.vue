<script setup lang="ts">
import {computed} from "vue";
const props = defineProps(["description"]);

const description = computed(() => props.description.toLowerCase())

</script>

<template>
    <h3>
      Hello {{description}} - From E
    </h3>
</template>

<style scoped>

h3 {
  color: darkgoldenrod;
  padding: 1em;
}
</style>
