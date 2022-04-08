<script setup lang="ts">
const props = defineProps(["description"]);
const {description} = props;

</script>

<template>
  <h2>Component A</h2>
  <p>This give the error</p>
  <p>

    "severity": 8,
    "message": "Getting a value from the `props` in root scope of script setup will cause the value to lose
    reactivity.",
    "source": "eslint",
    "startLineNumber": 3,
    "startColumn": 7,
    "endLineNumber": 3,
    "endColumn": 20
    }]
  </p>
  <p>As you can see it's not reactive</p>
  <pre>
  const {description} = props;
</pre>
  <h3>
    {{description}}
  </h3>
</template>

<style scoped>

h3 {
  color: darkgreen;
  padding: 1em;
}
</style>
