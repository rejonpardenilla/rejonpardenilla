<template>
  <div id="skills" class="mb-5">
    <h3 class="mb-1">Skills</h3>

    <skill-item name="Ruby on Rails" progress="94%"/>
    <skill-item name="Twitter Bootstrap" progress="98%"/>
    <skill-item name="Vue.js" progress="60%"/>
    <skill-item name="UI/UX Design" progress="80%"/>

  </div>  
</template>

<script>
import SkillItem from './SkillItem'

export default {
  components: { SkillItem }
}
</script>

<style lang="scss" scoped>
@import "../app";

#skills {
  margin-top: 5rem;

  h3 {
    color: $blue;
  }
}
</style>
