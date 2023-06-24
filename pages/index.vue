<script setup>
  const counter = useState('counter')
</script>

<template>
  <div>
    <h1>Welcome to my homepage</h1>
    <NuxtLink to="/about">About Page</NuxtLink>
    <p>Counter: {{ counter }}</p>
    <TtlViewer/>
  </div>
</template>
