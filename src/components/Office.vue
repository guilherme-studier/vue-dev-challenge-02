<template>
  <div class="offices">
    <div class="office">
      <div class="office-img">
        <img :src="img" alt="">
      </div>
      <p>{{ name }}</p>
    </div>
    <div class="office-office">
      <p>{{ office }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Office',
  props: {
    name: {
      type: String,
      default: ''
    },
    office: {
      type: String,
      default: ''
    },
    img: {
      type: String,
      default: '',
    },
    paddingTop: {
      type: Boolean,
      default: null,
    }
  }
}
</script>

<style>
  .offices {
    max-width: 264px;
    height: 500px;
    display: flex;
  }

  .office {
    width: 238px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }

  .office img {
    width: 100%;
  }

  .office p {
    font-family: 'Poppins', sans-serif;
    font-style: normal;
    text-align: initial;
    font-weight: 600;
    font-size: 18px;
    line-height: 27px;

    margin-block: 0;
    margin-top: 15px;
  }

  .office-office {
    width: 12px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    margin-left: 10px;
  }

  .office-office p {
    font-family: 'PT Serif', serif;
    font-style: normal;
    font-weight: bold;
    font-size: 12px;
    line-height: 16px;

    text-transform: uppercase;
    transform: rotate(90deg);
    
    margin-block: 0;
    white-space: nowrap;
  }

  @media (max-width: 600px) {
    .office {
      width: 138px;
    }

    .office p {
      font-size: 14px;
    }

    .offices {
      width: 156px;
      height: 261px;
      margin-bottom: 64px;
    }

    .office-office {
      margin-left: 6.28px;
    }

    .office-office p {
      font-size: 10px;
    }
  }
</style>