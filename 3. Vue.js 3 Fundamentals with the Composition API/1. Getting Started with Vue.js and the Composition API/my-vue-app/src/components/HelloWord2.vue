<script setup>
import { ref } from 'vue'

const header = ref('Shopping List App')
const items = ref({
  'data - 1':{id: 1, label: "10 party hats"},
  'data - 2':{id: 2, label:"2 board games"},
  'data - 3':{id: 3, label: "20 cups"}

}
  )
</script>

<template>
  <h1>{{ header }}</h1>
  <ul v-for="({id, label}, index) in items" :key="id">
    <li >
      {{label}}
      
    </li>
    <li >
      {{index}}
      
    </li>
  </ul>
</template>