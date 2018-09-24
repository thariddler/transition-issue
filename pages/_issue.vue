<template>
  <div>
    <h1>issue page</h1>
    <h1>issue page</h1>
    <h1>issue page</h1>
    <h1>issue page</h1>
    <h2>{{ data }}</h2>
  </div>
</template>

<script>
export default {
  props: [],
  validate ({ params, store, redirect }) {
    if (params.issue.charAt(0) !== '@') {
      redirect(`/@${params.issue}`)
    } else {
      return true
    }
  },
  async asyncData ({ params, query, store, error }) {
    try {
      setTimeout(() => {
        return {
          data: 'Hello, I am issue'
        }
      }, 300)
    } catch (err) {
      error({
        statusCode: 404,
        message: 'Oops!'
      })
    }
  },
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

</style>
