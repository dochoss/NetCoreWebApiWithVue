<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>

    <pre>{{ weather }}</pre>
  </div>
</template>

<script>
import axios from 'axios'
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data () {
    return {
      weather: []
    }
  },
  async mounted () {
    const res = await axios.get('weatherforecast')
    this.weather = res.data
  }
}
</script>
