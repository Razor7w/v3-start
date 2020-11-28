<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <router-view :key="key"/>
  </div>
</template>

<script>
export default {
  data () {
    return {
      key: this.$route.fullPath
    }
  },
  setup (props) {
    console.log(props)
    // const key = $route.fullPath
    return {
      // key
    }
  },
  mounted () {
    // console.log(this.$route.fullPath)
  }
}
</script>

<style lang="stylus">
#app
  font-family Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px
</style>
