<template>
  <section>
    <h1 class="main-title">Mes vacances en Suède</h1>
    <section class="pictures">
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
      <card :image="image" />
    </section>
  </section>
</template>

<script>
export default {
  data() {
    return {
      image: {
        src: 'abc.jpg',
      },
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
