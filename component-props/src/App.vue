<script setup>
import Count from './components/Count.vue';
import HelloWorld from './components/HelloWorld.vue';
const count1 = ref(0)
const count2 = ref(0)
const count3 = ref(0)
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <Count v-model="count1" :increaseNum="1" />
  <Count v-model="count2" :increaseNum="2" />
  <Count  v-model="count3" :increaseNum="3"/>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
