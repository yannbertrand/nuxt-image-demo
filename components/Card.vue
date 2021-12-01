<template>
  <article class="picture">
    <h2 class="img-src">{{ image.src }}</h2>
  </article>
</template>

<script>
export default {
  props: {
    image: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style scoped>
.picture {
  width: 460px;
  height: 400px;
  border: 1px solid black;
  background-color: white;
  box-shadow: 2px 5px 16px 0px #0b325e, 5px 5px 15px 5px rgba(0, 0, 0, 0);
  border-radius: 4px;
  margin: 10px;
  padding: 10px;
}

.picture h2 {
  margin: 0;
}

.img-src {
  font-family: 'Comic sans MS', serif;
}
</style>
