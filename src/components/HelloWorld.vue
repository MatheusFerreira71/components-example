<template>
  <div class="hello">
  <button @click="showUsername = !showUsername">Toggle Username</button>
    <div v-if="showUsername">
      <BigYellowUsername username="MatheusFerreira71"></BigYellowUsername>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    BigYellowUsername: () => import(/* webpackChunkName: "BigYellowUsername" */'./BigYellowUsername.vue')
  },
  data () {
    return {
      showUsername: false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
