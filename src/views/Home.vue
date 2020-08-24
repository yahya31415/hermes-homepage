<template>
  <div class="home">
    <section id="cover" class="d-flex flex-column justify-center align-center">
      <h1>Hermes</h1>
      <h3>E-commerce for everybody</h3>
      <CoverVideo />
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import CoverVideo from '@/components/CoverVideo.vue';

export default {
  name: 'Home',
  components: {
    CoverVideo,
  },
  mounted() {
    const sections = document.querySelectorAll('section');
    for (let i = 0; i < sections.length; i += 1) {
      sections[i].style.height = `${window.innerHeight}px`;
    }
  },
};
</script>

<style lang="scss">
.home {
  #cover {
    position: relative;
    h1,h3 {
      font-size: 8em;
      color: #FFF;
      z-index: 1;
      position: relative;
      line-height: 0.9;
    }
    h3 {
      font-size: 2.2em;
    }
  }
}
</style>
