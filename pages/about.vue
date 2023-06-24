<script setup>
  const counter = useState('counter')
</script>

<template>
  <div>
    <div>
      <h1>About me</h1>
      <NuxtLink to='/'>Home Page</NuxtLink>
    </div>
    <div>
      Counter: {{ counter }}
      <button @click="counter++">
        +
      </button>
      <button @click="counter--">
        -
      </button>
      <CounterMultiplier/>
    </div>
  </div>
</template>
