<template>
  <input type="text" :value="password"/>
  <button @click="generate">Generate Password</button>
</template>

<script>
export default {
  data () {
    return {
      password: 'password'
    }
  },
  methods: {
    generate () {
      this.password = Math.random().toString(36).slice(-8)
    }
  }
}
</script>

<style scoped lang="scss">

</style>
