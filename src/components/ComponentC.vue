<script setup lang="ts">
import {toRef} from "vue";

const props = defineProps(["description"]);
const description = toRef(props.description,"desc");

</script>

<template>
    <h3>
      Hello {{description}} - From C
    </h3>
</template>

<style scoped>

h3 {
  color: darkred;
  padding: 1em;
}
</style>
