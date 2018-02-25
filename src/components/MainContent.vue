<template>
  <div class="col-12 col-md-7 col-sm-6 col-lg-8 pt-5 pb-5" id="main-content">
    <div class="container">
      <content-info title="Summary" class="slide-right one">
        I’m a Jr. Web Developer currently coursing 6th semester of Software
        Engineering in the Facultad de Matemáticas in the Universidad Autónoma
        de Yucatán and I’m looking for an job in frontend or backend development.
      </content-info>

      <content-info title="Experience" class="slide-right two">
        <b>June 2017 - Present</b>: Ruby on Rails developer at CoDN. <br>
        <b>March 2017 - Present</b>: Laravel and Vuejs developer at a personal startup. <br>
        <b>February 2017</b>: Offer a firebase introductory course for Workshop Technology
          group organized by students of the Facultad de Matemáticas UADY. <br>
        <b>October 2016</b>: Second place at App Challenge 3 organized by the Facultad de Matemáticas UADY. <br>
      </content-info>

      <content-info title="Projects" class="slide-right three">
        <b>December 2017 - Present</b>: Hidrotanques admin panel development with Ruby on Rails for CoDN. <br>
        <b>September - December 2017</b>: Pay Inspector (payinspector.com) maintenance with Ruby on Rails for CoDN. <br>
        <b>June - September 2017</b>: Observatorio Costero UNAM Sisal (ocse.mx) development with Ruby on Rails for CoDN. <br>
        <b>March - May 2017</b>: A music service API made in Laravel for the API RESTful course. <br>
        <b>February 2016</b>: A to-do web app made in Foundation and Jquery for personal use. <br>
        <b>December 2016</b>: Tweet Analizer made in PHP for the Data Structures course. <br>
        <b>March - May 2016</b>: Tic Tac Toe game for the Software Design course. <br>
      </content-info>

      <content-info title="Education">
        <b>University</b>: Facultad de Matemáticas, Universidad Autónoma de Yucatán. <br>
        <b>Degree</b>: Software Engineering (graduating in 2019). <br>
        <b>Completed credits</b>: 73%. <br>
        <b>Grade point average</b>: 79/100. <br>
      </content-info>

      <content-info title="Strenghts">
        Frontend development with a vast set of tools. <br>
        UI/UX design with Sketch App. <br>
        Backend development with Ruby on Rails and PostgreSQL. <br>
        Object Oriented Programming with Ruby, PHP and Javascript. <br>
        Functional and asynchronous Javascript ES6. <br>
        Good comunication and interpersonal skills. <br>
        Problem solving and analysis skills. <br>
      </content-info>
    </div>
  </div>
</template>

<script>
import ContentInfo from './ContentInfo'

export default {
  components: { ContentInfo }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "../app";

#main-content {
  background-color: $light;
  color: $dark;
  text-align: left;
  border-top-right-radius: $resume-card-radius;
  border-bottom-right-radius: $resume-card-radius;

  @include media-breakpoint-down(sm) {
    border-top-left-radius: $resume-card-radius;
    border-bottom-left-radius: $resume-card-radius;
  }

}
</style>
