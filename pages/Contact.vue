<template>
  <div class="contact">
    <Navbar />
    <div class="contact__heading container-fluid">
      <div class="container">
        <h3>Contact Us</h3>
        <p>Reach out to us today and get your queries resolved.</p>
      </div>
    </div>
    <div class="contact__body container-fluid">
      <div class="container">
        <div class="row">
          <div class="contact__details container">
            <div class="details__card d-flex jusity-content-between">
              <div class="icon__holder">
                <font-awesome-icon :icon="['fa', 'phone']" />
              </div>
              <div class="details__body">
                <small>WE ARE ON 08:00 AM - 10:00 P.M</small>
                <p>Call : 0715 763 362</p>
              </div>
            </div>
            <div class="details__card d-flex jusity-content-between">
              <div class="icon__holder">
                <font-awesome-icon :icon="['fa', 'envelope']" />
              </div>
              <div class="details__body">
                <small>SEND US EMAIL ON</small>
                <p>globalexport1courierservicesx@gmail.com</p>
              </div>
            </div>
            <div class="details__card d-flex jusity-content-between">
              <div class="icon__holder">
                <font-awesome-icon :icon="['fa', 'home']" />
              </div>
              <div class="details__body">
                <small>MEET US AT</small>
                <p>Allen Avenue, Ikeja, Lagos, Nigeria</p>
              </div>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-12">
            <form action="">
              <div class="row">
                <div class="col-md-4">
                  <div class="form-group">
                    <label for="name">Name</label>
                    <input v-model="name" type="text" class="form-control" />
                  </div>
                  <div class="form-group">
                    <label for="email">Email</label>
                    <input v-model="email" type="text" class="form-control" />
                  </div>
                  <div class="form-group">
                    <label for="name">Subject</label>
                    <input v-model="subject" type="text" class="form-control" />
                  </div>
                </div>
                <div class="col-md-8">
                  <div class="form-group">
                    <label for="message">Messge</label>
                    <textarea
                      id=""
                      v-model="message"
                      name="message"
                      cols="30"
                      rows="6"
                      class="form-control"
                    ></textarea
                    ><br />
                    <button type="submit" class="contact__btn">
                      Send Message
                    </button>
                  </div>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style lang="scss" scoped>
.contact__heading {
  background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
    url('../assets/images/banner.jpg');
  background-size: cover;
  background-position: center;
  width: 100%;
  padding: 5rem 0;
  color: #fff;
  h3 {
    font-weight: bold;
    padding-top: 5rem;
  }
  p {
    font-size: 0.9rem;
    opacity: 0.9;
  }
}

.contact__body {
  background: #f5f5f5;
  .contact__details {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    grid-gap: 30px;
    margin-top: 5rem;
    margin-bottom: 3rem;
    .details__card {
      background: #fff;
      .icon__holder {
        background: #052c7d;
        padding: 1rem 1.4rem;
        color: #fff;
      }
      .details__body {
        padding: 0.2rem 0.7rem;
        small {
          font-size: 0.7rem;
        }
        p {
          font-size: 0.8rem;
        }
      }
    }
  }
  form {
    background: #fff;
    margin: 4rem 0;
    padding: 2rem;
    border-radius: 3px;
    label {
      font-size: 0.8rem;
      color: #2b2b2b;
      opacity: 0.8;
    }
    input {
      background: #f5f5f5;
      height: 2.7rem;
      border-radius: 1px;
      font-size: 0.9rem;
      box-shadow: none !important;
    }
    textarea {
      box-shadow: none !important;
      background: #f5f5f5;
    }
    .contact__btn {
      background: #052c7d;
      color: #fff;
      border: none;
      padding: 0.8rem 3rem;
      font-size: 0.85rem;
    }
  }
}
</style>
