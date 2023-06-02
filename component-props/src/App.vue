<script setup>
import { ref } from 'vue';
import HelloWorld from './components/HelloWorld.vue';
const count1 = ref(0)
const handleIncreaseCount1 = () => {
  count1.value +=
  1
} 
const count2 = ref(0)
const handleIncreaseCount2 = () => {
  count2.value +=
  2
}
const count3 = ref(0)
const handleIncreaseCount3 = () => {
  count3.value +=
  3
} 
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
  <div class="count" @click="handleIncreaseCount1">{{ count1 }}</div>
  <div class="count" @click="handleIncreaseCount2">{{ count2 }}</div>
  <div class="count" @click="handleIncreaseCount3">{{ count3 }}</div>
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

.count {

}
</style>
