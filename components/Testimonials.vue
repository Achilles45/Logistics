<template>
  <div class="testimonial">
    <div class="container">
      <div class="row">
        <div class="col-12 heading text-center">
          <small>What People Says About Us</small>
          <h1>CUSTOMER REVIEWS</h1>
        </div>
      </div>
      <div class="testimonial__wrapper text-center">
        <div class="testimonial__card">
          <img src="../assets/images/quote.svg" class="icon" alt="" />
          <div class="text">
            <img src="../assets/images/review.png" class="review" alt="" />
            <p>
              Their storage facilities are top notch... I got my parcel without
              a single scratch or dent to it. It was like they were handling it
              as though they were handling an egg.
            </p>
          </div>
        </div>
        <div class="testimonial__card">
          <img src="../assets/images/quote.svg" class="icon" alt="" />
          <div class="text">
            <img src="../assets/images/review2.png" class="review" alt="" />
            <p>
              Their sshipping services are worth the prices and they just don't
              deliver, they deliver on time and their staff are very polite.
            </p>
          </div>
        </div>
        <div class="testimonial__card">
          <img src="../assets/images/quote.svg" class="icon" alt="" />
          <div class="text">
            <img src="../assets/images/review3.png" class="review" alt="" />
            <p>
              I was actually satisfied. I got all my items in record time and
              the tracking process was very efficient.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.testimonial {
  padding: 6rem 0;
  .heading {
    small {
      font-weight: bold;
      color: #052c7d;
    }
    h1 {
      font-weight: bold;
      padding-top: 0.5rem;
      font-size: 2.4rem;
      color: #272727;
    }
  }
  .testimonial__wrapper {
    margin-top: 3rem;
    display: flex;
    overflow-x: scroll;
    overflow-y: hidden;
    align-items: center;
    ::-webkit-scrollbar {
      height: 1px; /* height of horizontal scrollbar ← You're missing this */
      width: 1px; /* width of vertical scrollbar */
      color: red;
    }
    .testimonial__card {
      display: inline-block;
      margin: 0 0.3rem;
      min-width: 550px;
      padding: 3rem;
      position: relative;
      .icon {
        position: absolute;
        left: 20px;
        top: 20px;
        max-width: 25px;
        height: auto;
      }
      .review {
        border-radius: 50px;
        max-width: 70px;
        height: auto;
      }
      p {
        padding-top: 1rem;
        font-size: 0.9rem;
        color: #2b2b2b;
      }
    }
  }
}
</style>
