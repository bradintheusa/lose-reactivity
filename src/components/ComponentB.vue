<script setup lang="ts">
import {toRefs} from "vue";
const props = defineProps(["description","ladder"]);

const {description} = toRefs(props);
</script>

<template>
    <h3>
      Hello {{description}} - From B
    </h3>
</template>

<style scoped>

h3 {
  color: navy;
  padding: 1em;
}
</style>
