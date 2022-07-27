
<template>
<h1>Ninja Reaction Timer</h1>
<NinjaTimerBlock />
<ReactionTimerResult/>
</template>

<script>
import NinjaTimerBlock from './components/ReactionTimerBlock.vue'
import ReactionTimerResult from './components/ReactionTimerResult.vue'
export default {
  name: 'App',
  components: {
       NinjaTimerBlock,
       ReactionTimerResult
    },
  data() {
    return {
      title: "My First Vue App :)"
    }
  },
  methods: {
    handleInput() {
      console.log(this.$refs.name)
      this.$refs.name.classList.add('active')
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
