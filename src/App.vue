<template>
  <div id="app">
    <div class="row justify-content-center">
      <div class="col-9">
        <div class="row" id="resume-card">
          <sidebar />
          <main-content />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar'
import MainContent from './components/MainContent'

export default {
  components: {
    Sidebar,
    MainContent
  }
}
</script>

<style lang="scss">
@import "app";

#app {
  font-family: $font-family-sans-serif;
}

#resume-card {
  background-color: $light;
  margin-top: 3rem;
  margin-bottom: 3rem;
  border-radius: $resume-card-radius;
  box-shadow: 10px 10px 6px -6px #777;
}
</style>
