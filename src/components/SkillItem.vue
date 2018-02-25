<template>
  <div id="skill-item">
    <h5 class="text-left mb-1">{{this.name}}</h5>

    <div id="skill-bar" class="mb-3">
      <div id="progress" :style="{width: this.progress}">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['name', 'progress']
}
</script>

<style lang="scss" scoped>
@import "../app";

#skill-item {
  h5 {
    font-weight: 100;
  }
}

#skill-bar {
  background-color: $light;
  height: 0.6rem;
  border-radius: 0.6rem;

  #progress {
    background-color: $blue;
    height: 0.6rem;
    border-radius: 0.6rem;  
  }
}
</style>
