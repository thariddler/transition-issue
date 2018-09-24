<template>
  <header>
    <nav>
      <ul>
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/qqq">Issue</nuxt-link></li>
        <li><nuxt-link to="/ok">OK</nuxt-link></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  props: [],
  data () {
    return {
      //
    }
  },
  methods: {
    //
  }
}
</script>

<style lang="stylus" scoped>
header
  width 100%
ul
  display flex
  justify-content center
  width 100%
  text-decoration none
  list-style none

li
  margin 1em
</style>
