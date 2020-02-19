<template>
  <div class="navbar__wrapper container-fluid">
    <div class="container">
      <div
        class="navbar__contents d-flex justify-content-between align-items-center"
      >
        <div class="navbar__logo pt-2">
          <nuxt-link to="/" class="logo"
            ><h4>
              <font-awesome-icon :icon="['fa', 'globe']" /> Logistics
            </h4></nuxt-link
          >
        </div>
        <div class="navbar__links">
          <ul class="d-flex navbar__items justify-content-between pt-3">
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/">About Us</nuxt-link></li>
            <li><nuxt-link to="/">Contact Us</nuxt-link></li>
            <li><nuxt-link to="/">Track your goods</nuxt-link></li>
            <li>
              <nuxt-link to="/" class="quote__btn">Request a Quote</nuxt-link>
            </li>
          </ul>
        </div>
        <div class="navbar__toggler" @click="toggleNav()">
          <font-awesome-icon :icon="['fa', 'bars']" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    toggleNav() {
      const navbarToggler = document.querySelector('.navbar__toggler')
      const nav = document.querySelector('.navbar__items')
      navbarToggler.addEventListener('click', () => {
        nav.classList.toggle('show__nav')
      })
    }
  }
}
</script>

<style lang="scss" scoped>
.navbar__wrapper {
  background: #fff;
  box-shadow: 3px 0px 3px rgba(0, 0, 0, 0.4);
  color: #fff;
  padding: 0.7rem 0;
  position: fixed;
  z-index: 100;
  .logo {
    color: #fff;
    font-weight: bold;
    text-decoration: none !important;
    color: #2ecc71;
    opacity: 0.7;
  }
  ul {
    li a {
      text-decoration: none;
      color: #052c7d;
      text-transform: uppercase;
      font-size: 0.8rem;
      opacity: 0.8;
      margin: 0 0.6rem;
      font-weight: bold;
      &:hover {
        color: #2ecc71;
        transition: all ease-in-out 0.5s;
      }
    }
    .quote__btn {
      background: #2ecc71;
      padding: 1rem 2rem;
      border-radius: 3px;
      opacity: 1 !important;
      color: #fff;
      font-weight: normal;
      &:hover {
        color: #fff !important;
        padding: 1rem 2.5rem;
        transition: all ease-in-out 0.5s;
      }
    }
  }
  .navbar__toggler {
    color: #2b2b2b;
    display: none;
  }
}
//MEDIA QUERIES
@media only screen and (max-width: 1000px) {
  .navbar__toggler {
    display: block !important;
    cursor: pointer;
  }
  ul {
    background: #000;
    flex-direction: column;
    position: absolute;
    padding: 23rem 2rem;
    left: 0;
    top: 100%;
    line-height: 4rem;
    display: none !important;
    li a {
      color: #fff !important;
      line-height: 5rem;
      margin-top: 2rem !important;
    }
  }
  .show__nav {
    display: block !important;
    transition: all ease-in-out 0.5s;
  }
}
</style>
