<template>
  <div class="track">
    <Navbar />
    <div class="track__heading">
      <div class="container">
        <h2>Need any logistics service?</h2>
        <p>Reach out to us today for all your professional shipping needs</p>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <form action="">
            <div class="row">
              <div class="col-md-6">
                <div class="form-group">
                  <label for="freight">Freight Type</label>
                  <select
                    id=""
                    v-model="type"
                    name="select"
                    class="form-control"
                  >
                    <option value="d">Choose a type</option>
                    <option value="Road">Road Transportation</option>
                    <option value="Air">Air Transportation</option>
                    <option value="Sea">Sea Transportation</option>
                    <option value="Warehousing">Warehousing</option>
                  </select>
                </div>
                <div class="form-group">
                  <label for="city">Departure</label>
                  <input v-model="city" type="text" class="form-control" />
                </div>
                <div class="form-group">
                  <label for="city">Destination</label>
                  <input
                    v-model="destination"
                    type="text"
                    class="form-control"
                  />
                </div>
                <div class="form-group">
                  <label for="freight">Freight Type</label>
                  <select
                    id=""
                    v-model="type"
                    name="terms"
                    class="form-control"
                  >
                    <option value="EXW">EXW</option>
                    <option value="FCA">FCA</option>
                    <option value="CPT">CPT</option>
                    <option value="CIP">CIP</option>
                  </select>
                </div>
                <div class="form-group">
                  <label for="weight">Gross Weight (KG)</label>
                  <input v-model="weight" type="text" class="form-control" />
                </div>
              </div>
              <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Your Full Name</label>
                  <input v-model="name" type="text" class="form-control" />
                </div>
                <div class="form-group">
                  <label for="email">Your Email Address</label>
                  <input v-model="email" type="text" class="form-control" />
                </div>
                <div class="form-group">
                  <label for="instruction">Special Instruction</label>
                  <textarea
                    id=""
                    v-model="instruction"
                    name=""
                    cols="30"
                    rows="6"
                    class="form-control"
                  ></textarea>
                </div>
                <br />
                <button type="sumit" class="request__btn">Request Quote</button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <br /><br />
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar'
import Footer from '~/components/Footer'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style lang="scss" scoped>
.track {
  background: #fff;
  .track__heading {
    background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
      url('../assets/images/banner.jpg');
    background-size: cover;
    background-position: center;
    width: 100%;
    padding: 5rem 0;
    h2 {
      color: #fff;
      padding-top: 5rem;
      text-transform: capitalize;
    }
    p {
      font-size: 0.85rem;
      opacity: 0.8;
      color: #fff;
    }
  }
  form {
    margin-top: 5rem;
    margin-bottom: 5rem;
    label {
      color: #545454;
      font-size: 0.84rem;
      opacity: 0.9;
      padding-bottom: 0.5rem;
    }
    input,
    select {
      width: 100%;
      height: 2.8rem;
      background: #fff;
      box-shadow: none !important;
      border-radius: 0px;
      margin-bottom: 1rem;
      border: 1px solid #ccc;
    }
    .request__btn {
      background: #052c7d;
      color: #fff;
      border-radius: 3px;
      padding: 0.9rem 3rem;
      border: none;
      font-size: 0.85rem;
      &:hover {
        background: #2ecc71;
        transition: all ease-in 0.5s;
      }
    }
  }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px) {
  .track__heading {
    padding: 3rem 0;
  }
  .form {
    padding: 3rem 0rem !important;
  }
}
</style>
