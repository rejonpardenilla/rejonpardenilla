<template>
  <div class="col-12 col-md-5 col-sm-6 col-lg-4" id="sidebar">
    <div class="container">
      <img src="@/assets/photo.png" alt="photo" class="appear-photo">
      <h2 class="slide-left one">Daniel Rejón Pardenilla</h2>
      <h5 class="mb-5 slide-left two">Software Engineer</h5>
      <contact/>
      <skills />
      <technologies />
    </div>
  </div>
</template>

<script>
import Contact from './Contact'
import Skills from './Skills'
import Technologies from './Technologies'

export default {
  components: {
    Contact,
    Skills,
    Technologies
  }
}
</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap.scss";
@import "../app";

#sidebar {
  background-color: $dark;
  color: $light;
  text-align: center;
  border-top-left-radius: $resume-card-radius;
  border-bottom-left-radius: $resume-card-radius;

  @include media-breakpoint-down(sm) {
    border-top-right-radius: $resume-card-radius;
    border-bottom-right-radius: $resume-card-radius;
  }

  h1, h2, h3, h4, h5 {
    color: $blue
  }

  h5 {
    font-style: italic;
    font-weight: 300;
  }

  img {
    height: 8rem;
    margin-top: 2.5rem;
    margin-bottom: 2rem;
    transition: all .4s ease-in-out;
  }

  img:hover {
    transform: scale(1.5);
    margin-top: 5rem;
    margin-bottom: 4rem;
  }
}
</style>
