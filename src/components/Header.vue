<template>
  <header>
    <div class="header-title">
      <h1>The creative crew</h1>
    </div>
    <div class="header-subtitle">
      <h2>Who we are</h2>
      <p>
        We are team of creatively diverse. driven. innovative individuals working in various locations from the world
      </p>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style>
  header {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-top: 98px;
  }

  header div {
    flex: 1 1 400px;
  }

  header .header-title {
    width: 303px;
    text-align: left;
  }

  header .header-title h1 {
    font-family: 'PT Serif', serif;
    font-weight: 700;
    font-size: 36px;

    margin-block: 0;
  }

  header .header-subtitle {
    width: 439px;
    text-align: left;
  }

  header .header-subtitle h2 {
    font-family: 'Poppins', sans-serif;
    text-transform: uppercase;
    font-weight: 600;
    font-size: 18px;

    margin-block: 0;
  }

  header .header-subtitle p {
    font-family: 'Poppins', sans-serif;
    line-height: 27px;
    font-weight: 400;
    font-size: 18px;

    margin-block: 0;
  }

  @media (max-width:600px) {
    header {
      margin-top: 59px;
    }
    
    header .header-subtitle {
      width: 333px;
      margin-top: 38px;
      text-align: left;
    }
    header .header-subtitle p {
      font-size: 14px;
      width: 333px;
    }
  }
</style>