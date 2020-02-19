<template>
  <div class="banner">
    <div class="container">
      <div class="row">
        <div
          class="col-md-6 col-lg-6
        col-sm-12 col-xs-12 banner__text"
        >
          <h1>Your logistics partner of choice</h1>
          <p>
            We abstract away all form logistics for your business so you can
            focus on what really matters to your businss. From sea, air and
            road, we've got you coverd.
          </p>
          <nuxt-link to="/" class="banner__btn">Request Our Services</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.banner {
  background: linear-gradient(rgba(4, 9, 30, 0.8), rgba(4, 9, 30, 0.8)),
    url('../assets/images/slider-1.jpg');
  background-size: cover;
  background-position: center;
  height: 95vh;
  width: 100%;
  position: relative;
  .banner__text {
    position: absolute;
    top: 38%;
    transform: translateX(50%, -50%);
    h1 {
      color: #fff;
      text-transform: uppercase;
      font-weight: 900;
      line-height: 1.3;
      text-shadow: rgba(0, 0, 0, 0.15) -2px 4px 18px;
      font-size: 2.7rem;
      transform-origin: 50% 50% 0px;
      //   opacity: 0.9;
      padding-bottom: 1rem;
    }
    p {
      color: #fff;
      opacity: 0.7;
      padding-bottom: 2rem;
      font-size: 0.9rem;
      line-height: 1.8;
    }
    .banner__btn {
      background: #052c7d;
      color: #fff;
      text-decoration: none;
      border-radius: 4px;
      padding: 1.4rem 4rem;
      font-size: 0.82rem;
      &:hover {
        background: #1ecf68;
        transition: all ease-in-out 0.05;
      }
    }
  }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px) {
  .banner {
    height: 100vh;
    .banner__text {
      h1 {
        font-size: 2rem !important;
      }
    }
  }
}
</style>
