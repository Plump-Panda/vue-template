<template>
  <div class="main">
    <div class="image-container">
      <section class="image-row">
        <Logo :description="test" :image="github"/>
        <Logo :description="test" :image="cypress"/>
        <Logo :description="test" :image="codefresh"/>
      </section>
      <section class="image-row">
        <Logo :description="test" :image="java"/>
        <Logo :description="test" :image="mixpanel"/>
        <Logo :description="test" :image="docker"/>
      </section>
      <section class="image-row">
        <Logo :description="test" :image="vue"/>
        <Logo :description="test" :image="flask"/>
        <Logo :description="test" :image="linux"/>
      </section>
    </div>
  </div>
</template>

<script>
import Logo from './Logo.vue';
import constants from '../constants/constants.js';

export default {
  name: 'MainPage',
  components: {
    Logo,
  },
  props: {
    msg: String
  },
  data: function() {
    return {
      test: 'test description',
      codefresh: constants.images.codefresh,
      cypress: constants.images.cypress,
      docker: constants.images.docker,
      flask: constants.images.flask,
      github: constants.images.github,
      java: constants.images.java,
      linux: constants.images.linux,
      mixpanel: constants.images.mixpanel,
      vue: constants.images.vue,
    }
  },
}
</script>

<style scoped>
  .image-row {
    display: flex;
  }
</style>
