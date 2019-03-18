<template>
  <div id="app">
    <section class="hero is-fullheight mainhero">
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="columns is-centered is-vcentered">
            <div class="column is-two-fifth white-seperator">
              <h1 class="custom-subtitle">Mauritius, June 10</h1>
              <h2 class="custom-title">Switch Conference</h2>
            </div>
            <div class="column is-two-fifth">
              <img class="logo-hero" :src="require('./assets/logo.png')">
            </div>
          </div> <!-- Columns End -->
          <button class="button custom-button">
              Call For Sponsors
          </button>
        </div>
      </div>
    </section>
    <!-- <div class="hero">
      <h1>
        Switch Conference
        31st March & 1st June 2019
        Mauritius 🇲🇺
      </h1>
      <a href class="button">Call for sponsors</a>
    </div>-->
  </div>
</template>

<style lang="scss" scoped>

$mobile:400px;

.white-seperator{
    border-right: 4px solid white;

    @media only screen and (max-width:$mobile) {
    border: none;
  }
}

.mainhero {
  background: url("./assets/img1.png") no-repeat fixed center;

  .hero-body {
    background: linear-gradient(180deg, rgba(39, 65, 143, 0.6) 0%, rgba(205, 93, 86, 0.6) 100%);
  }
}

.custom-button{
  margin-top:1rem;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  background: #27418F;
  border: 0px;
  border-radius: 4px;
  font-size: 1.5rem;
  color: white;
  font-family:"Ubuntu",sans-serif;
}

.custom-title{
font-family: Ubuntu;
font-weight: bold;
font-size: 6rem;
text-align: center;
color: #FFFFFF;
  @media only screen and (max-width:$mobile) {
    font-size: 3rem;
  }
}

.custom-subtitle{
  text-align:center;
  font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 36px;
line-height: normal;
color: #FFFFFF;

  @media only screen and (max-width:$mobile) {
    font-size: 1.5rem;
  }
}

.logo-hero {
  max-height:50%;
  max-width:50%;

  @media only screen and (max-width:$mobile) {
    margin-left: 4rem;
  }
}
</style>


<script>
export default {
  name: "app",
};
</script>