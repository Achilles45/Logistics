<template>
  <div class="app">
    <Navbar />
    <Banner />
    <Services />
    <Why />
    <Testimonials />
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Banner from '~/components/Banner.vue'
import Services from '~/components/Services.vue'
import Why from '~/components/Why.vue'
import Testimonials from '~/components/Testimonials.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    Banner,
    Services,
    Why,
    Testimonials,
    Footer
  }
}
</script>
