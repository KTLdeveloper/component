<script setup lang="ts">
import { defineEmits, defineProps } from 'vue';
interface Props {
    modelValue: Number
    increaseNum: Number
}
interface Emits {
    (e: 'update:modelValue', value: Number): void
}
const props = defineProps<Props>({
  modelValue: Number,
  increaseNum: Number
})

const emit = defineEmits<Emits>()

const handleClick= () => {
    const newValue = props.modelValue += props.increaseNum
    emit('update:modelValue', newValue)
}
</script>

<template>
  <div @click="handleClick">{{ modelValue }}</div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
