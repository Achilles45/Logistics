<template>
  <footer class="container-fluid">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <h3>Logistics</h3>
          <p>
            The Company was established to cater for domestic and commercial
            shipping world wide with our headquartered in and Branches all over
            the world.
          </p>
        </div>
        <div class="col-md-4">
          <h3>Useful Links</h3>
          <ul class="d-block justify-content-between flex-direction-column">
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/">About Us</nuxt-link></li>
            <li><nuxt-link to="/">Contact Us</nuxt-link></li>
            <li><nuxt-link to="/">Service request</nuxt-link></li>
            <li><nuxt-link to="/">Track your goods</nuxt-link></li>
          </ul>
        </div>
        <div class="col-md-4">
          <h3>Subscribe to our newsletter</h3>
          <form action="">
            <input
              type="email"
              class="form-control"
              placeholder="Email Address"
            /><br />
            <button type="submit" class="newsletter__btn">Subscribe</button>
          </form>
        </div>
      </div>
      <br />
      <hr />
      <small
        >&copy; All right reserved. Logistics, 2020. Terms and Conditions
        Apply</small
      >
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
footer {
  background: linear-gradient(rgba(4, 9, 30, 0.9), rgba(4, 9, 30, 0.9)),
    url('../assets/images/slider-1.jpg');
  background-size: cover;
  background-position: center;
  padding: 7rem 0;
  color: #fff;
  h3 {
    padding-bottom: 2rem;
    font-size: 1.3rem;
    text-transform: uppercase;
    opacity: 0.8;
  }
  p {
    font-size: 0.9rem;
    opacity: 0.7;
    line-height: 1.7;
  }
  form {
    input {
      height: 3rem;
      background: #f5f5f5;
      border-radius: 3px;
      box-shadow: none !important;
      opacity: 0.9;
      font-size: 0.9rem;
      padding: 0.3rem 0.5rem;
    }
    .newsletter__btn {
      background: #052c7d;
      color: #fff;
      padding: 1rem 2.5rem;
      border-radius: 50px;
      text-decoration: none;
      border: none;
      font-size: 0.9rem;
    }
  }
  small {
    opacity: 0.7;
  }
}
</style>
