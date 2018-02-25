<template>
  <div class="row justify-content-center mb-5">
    <div class="col-12 col-md-10 col-lg-8">
      <h3>{{this.title}}</h3>
      <p>
        <slot>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
          Adipisci deserunt accusamus deleniti expedita ut modi nam?
          Laborum officiis aut veniam perspiciatis error, totam, aperiam
          saepe atque eius, soluta eos delectus?
        </slot>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title']
}
</script>

<style lang="scss" scoped>
</style>
