<script setup lang="ts">
import {ref } from "vue";
import ComponentA from './components/ComponentA.vue'
import ComponentB from './components/ComponentB.vue'
import ComponentC from './components/ComponentC.vue'
import ComponentD from './components/ComponentD.vue'
import ComponentE from './components/ComponentE.vue'


const name = ref("World");
// const name = "World";

function changeText() {
  name.value = "Planet";
}

</script>

<template>
  <header>
    <h2>What's your name:</h2>
    <p>  <input type="text" v-model="name" >
    </p>
    <button @click="changeText">Click Me</button>

    <h3>Hello {{name}}</h3>
    <div class="wrapper">
      <ComponentA :description="name"  />
      <ComponentB :description="name"  />
      <ComponentC :description="name"  />
      <ComponentD :description="name"  />
      <ComponentE :description="name"  />
    </div>
  </header>

</template>

<style>
@import './assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

input {
  padding-bottom: 20px;
}

button {
  color: whitesmoke;
  background-color: navy;
  margin: 10px;
  padding: 10px;
  border-radius: 5px;
}

</style>
