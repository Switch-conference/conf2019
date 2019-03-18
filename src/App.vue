<template>
  <div id="app">
    <section class="hero is-fullheight mainhero">
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="columns is-centered is-vcentered">
            <div class="column is-two-fifth white-seperator">
              <h1 class="custom-subtitle">Mauritius, 31st March & 1st June 2019</h1>
              <h2 class="custom-title">Switch Conference</h2>
            </div>
            <div class="column is-two-fifth">
              <img class="logo-hero" :src="require('./assets/logo.png')">
            </div>
          </div>
          <!-- Columns End -->
          <a class="button is-large custom-button">Call For Sponsors</a>
        </div>
      </div>
    </section>
  </div>
</template>

<style lang="scss" scoped>
$mobile: 768px;

.white-seperator {
  border-right: 4px solid white;

  @media only screen and (max-width: $mobile) {
    border: none;
  }
}

.mainhero {
  background: url("./assets/img1.png") no-repeat fixed center;
  height: 100vh;
  display: flex;
  align-content: center;
  justify-content: center;

  .hero-body {
    background: linear-gradient(180deg, rgba(39, 65, 143, 0.6) 0%, rgba(205, 93, 86, 0.6) 100%);
  }
}

.custom-button {
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  background: #27418f;
  border: 4px solid #27418f;
  border-radius: 4px;
  font-size: 1.5rem;
  color:#ffffff;
  transition: all ease-in 0.2s;

  &:hover {
    background: transparent;
    color:#ffffff;
    border-color: #27418f;
  }
}

.custom-title {
  font-family: Lato;
  font-weight: bold;
  font-size: 48px;
  text-align: center;
  color: #ffffff;
  line-height: normal;
  @media only screen and (max-width: $mobile) {
    font-size: 3rem;
  }
}

.custom-subtitle {
  text-align: center;
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
  line-height: normal;
  color: #ffffff;

  @media only screen and (max-width: $mobile) {
    font-size: 1.5rem;
  }
}

.logo-hero {
  max-height: 50%;
  max-width: 50%;
}
</style>


<script>
export default {
  name: "app",
};
</script>