<template>
  <section>
    <h1 class="main-title">Mes vacances en Suède</h1>
    <section class="pictures">
      <card v-for="image of images" :key="image.src" :image="image" />
    </section>
  </section>
</template>

<script>
export default {
  data() {
    return {
      images: [
        {
          src: 'pictures/IMG_9240.jpeg',
        },
        {
          src: 'pictures/IMG_9335.jpeg',
        },
        {
          src: 'pictures/IMG_9401.jpeg',
        },
        {
          src: 'pictures/IMG_9413.jpeg',
        },
        {
          src: 'pictures/IMG_9432.jpeg',
        },
        {
          src: 'pictures/IMG_9443.jpeg',
        },
        {
          src: 'pictures/IMG_9447.jpeg',
        },
      ],
    }
  },
}
</script>

<style scoped>
.main-title {
  font-family: 'Gill Sans', sans-serif;
  font-size: 2rem;
}

.pictures {
  display: flex;
  flex-wrap: wrap;
}
</style>
