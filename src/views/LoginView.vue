<template>
    <div>
        <input type="text" v-model="output">
        <h1>{{ outputComputed }}</h1>
    </div>
</template>

<script setup lang="ts">
import { computed, ref } from 'vue';

const output = ref("")
const outputComputed = computed(() => output.value.toUpperCase())
</script>

<style scoped lang="scss">

</style>