<template>
    <div class="image-container">
        <img class="image" :src="require(`@/assets/${image}`)">
    </div>
</template>

<script>
export default {
  name: 'Logo',
  props: {
    description: String,
    image: String,
  }
}
</script>

<style scoped>
  .image {
    width: 5em;
  }
</style>

