<script setup>
import { ref } from 'vue'

const header = ref('Shopping List App')
</script>

<template>
  <h1>{{ header.toUpperCase() }}</h1>
  <h1>{{ header.toLocaleUpperCase() }}</h1>
  <input type="text" v-model="header">
</template>