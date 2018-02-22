<template>
  <div class="container mt-4 mb-5">
    <div class="row justify-content-center">
      <contact-link name="rejonpardenilla.com"
                    href="http://rejonpardenilla.com"
                    icon="globe" />
      <contact-link name="rejonpardenilla@gmail.com"
                    href="mailto:rejonpardenilla@gmail.com"
                    icon="envelope" />
      <contact-link name="github.com/rejonpardenilla"
                    href="http://github.com/rejonpardenilla"
                    icon="github-alt" />
      <contact-link name="linkedin.com/in/rejonpardenilla"
                    href="http://linkedin.com/in/rejonpardenilla"
                    icon="linkedin-square" />
      <contact-link name="+52 1 999 956 8778"
                    href="#"
                    icon="phone" />
    </div>
  </div>
</template>

<script>
import ContactLink from './ContactLink'

export default {
  components: { ContactLink }
}
</script>

<style lang="scss" scoped>
</style>
