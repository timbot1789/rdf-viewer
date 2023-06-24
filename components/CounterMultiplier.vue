<script setup>
  const counter = useState('counter', () => 45)
</script>

<template>
  <div>
    Counter from component: {{  counter }}
    <button @click="counter = counter * 2">double</button>
    <button @click="counter = counter / 2">halve</button>
  </div>
</template>
