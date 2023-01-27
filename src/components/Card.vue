<template>
  <section>
    <Office name="Bill Mahoney" office="Product owner" :img="photo1" />
    <Office name="Saba Cabrera" office="Art director" :img="photo2" paddingTop />
    <Office name="Shae Le" office="Tech Lead" :img="photo3" />
    <Office name="Bill Mahoney" office="Product owner" :img="photo4" />
    <Office name="Saba Cabrera" office="Art director" :img="photo5" paddingTop />
    <Office name="Shae Le" office="Tech Lead" :img="photo6" />
  </section>
</template>

<script>
import Office from './Office.vue';

import photo1 from '../assets/photo1.png';
import photo2 from '../assets/photo2.png';
import photo3 from '../assets/photo3.png';
import photo4 from '../assets/photo4.png';
import photo5 from '../assets/photo5.png';
import photo6 from '../assets/photo6.png';

export default {
  name: 'Card',
  data() {
    return {
      photo1: photo1,
      photo2: photo2,
      photo3: photo3,
      photo4: photo4,
      photo5: photo5,
      photo6: photo6,
    }
  },
  components: {
    Office,
  }
}
</script>

<style scoped>
  section {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }

  section div {
    flex: 1 1 156px;
  }

  section div:nth-child(3n+2) {
    padding-top: 80px;
  }

  @media(max-width: 800px) {
    section div:nth-child(3n+2) {
      padding-top: 0px;
    }
    
    section div:nth-child(2n) {
      padding-top: 55px;
      justify-content: end;
    }
  }

</style>