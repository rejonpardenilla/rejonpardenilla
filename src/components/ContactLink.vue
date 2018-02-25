<template>
  <div class="col-12 slide-left three" id="contact-link">
    <a :href="this.href" target="_blank">
      <icon :name="this.icon"></icon>
      {{this.name}}
    </a>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  props: ['icon', 'href', 'name'],
  components: {
    Icon
  }
}
</script>

<style lang="scss" scoped>
@import "../app";

#contact-link {
  a {
    color: $light;
    font-weight: 100;
    font-size: 15px;
  }

  svg {
    height: 12px;
    color: $blue;
  }
}
</style>
