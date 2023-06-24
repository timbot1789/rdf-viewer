<script setup>
  import Two from "two.js";
  const stage = ref(null);
  
  function initTwo() {
    const two = new Two({
      fullscreen:true
    }).appendTo(stage.value);

    const x = two.width * 0.5;
    const y = two.height * 0.5;
    const width = 100;
    const height = 100;
    const rect = two.makeRectangle(x, y, width, height);

    rect.fill = 'rgb(0, 200, 255)';
    two.update();
  }

  onMounted(() => {
    initTwo();
  })

</script>

<template>
  <div ref='stage' />
</template>
