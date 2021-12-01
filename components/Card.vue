<template>
  <article class="picture">
    <h2 class="image-title">{{ image.src }}</h2>
    <nuxt-img
      class="image-img"
      :src="image.src"
      width="403"
      height="302"
      alt=""
    />
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
  width: 403px;
  border: 1px solid black;
  background-color: white;
  box-shadow: 2px 5px 16px 0px #0b325e, 5px 5px 15px 5px rgba(0, 0, 0, 0);
  border-radius: 4px;
  margin: 10px;
  padding: 10px;
}

.picture .image-title {
  margin: 0;
  margin-bottom: 10px;
}

.picture .image-img {
  max-width: 100%;
}

.img-src {
  font-family: 'Comic sans MS', serif;
}
</style>
