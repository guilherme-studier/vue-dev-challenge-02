<template>
  <Header />
  <section>
    <Card />
  </section>
  <Footer />
</template>

<script>
import Header from '../components/Header.vue';
import Card from '../components/Card.vue';
import Footer from '../components/Footer.vue';

export default {
  name: 'Home',
  components: {
    Header,
    Card,
    Footer
  }
}
</script>

<style scoped>
  section {
    padding: 96px 0;
  }

  @media (max-width: 800px) {
    section {
      padding: 25px 0;
      width: 338px;
    }
  }
</style>