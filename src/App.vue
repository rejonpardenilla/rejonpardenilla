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

.slide-left.one {
  animation: slideInFromLeft 1s;
}
.slide-left.two {
  animation: slideInFromLeft 1.5s;
}
.slide-left.three {
  animation: slideInFromLeft 2s;
}
.slide-left.four {
  animation: slideInFromLeft 2.5s;
}

.slide-right.one {
  animation: slideInFromRight 1s;
}
.slide-right.two {
  animation: slideInFromRight 1.5s;
}
.slide-right.three {
  animation: slideInFromRight 2s;
}
.slide-right.four {
  animation: slideInFromRight 2.5s;
}

@keyframes slideInFromLeft {
  0% {
    transform: translateX(-100%);
  }
  100% {
    transform: translateX(0);
  }
}

@keyframes slideInFromRight {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(0);
  }
}

.appear-photo {
  animation: appearPhoto 2.5s;
}

@keyframes appearPhoto {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
