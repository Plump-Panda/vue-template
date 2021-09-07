<template>
    <div>
        <img :src="require(`@/assets/${image}`)">
        <section>
          {{description}}
        </section>
    </div>
</template>

<script>
export default {
  name: 'JobCard',
  props: {
    description: String,
    image: String,
  }
}
</script>

<style scoped>
</style>

