<template>
  <div class="main">
    <JobCard :description="test" :image="codefresh"/>
    <JobCard :description="test" :image="cypress"/>
  </div>
</template>

<script>
import JobCard from './JobCard.vue';
import constants from '../constants/constants.js';

export default {
  name: 'MainPage',
  components: {
    JobCard,
  },
  props: {
    msg: String
  },
  data: function() {
    return {
      test: 'test description',
      codefresh: constants.images.codefresh,
      cypress: constants.images.cypress,
    }
  },
}
</script>

<style scoped>
</style>
