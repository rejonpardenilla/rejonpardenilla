<template>
  <div class="col-12" id="contact-link">
    <a :href="href" target="_blank">
      <icon :name="icon"></icon>
      {{name}}
    </a>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  props: ['icon', 'href', 'name'],
  data () {
    return {
      name: this.name,
      href: this.href,
      icon: this.name
    }
  },
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
