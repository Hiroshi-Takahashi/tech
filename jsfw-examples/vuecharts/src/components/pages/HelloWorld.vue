<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <LineChart witdh='300' height='300' fill='#000000'></LineChart>
<!--
    <div>---computed---</div>
    <div>{{now}}</div>
-->
  </div>
</template>

<script>
import LineChart from '@/components/parts/LineChart'

export default {
  name: 'HelloWorld',
  components: {
    'LineChart': LineChart
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  computed: {
    now: function () {
      console.log('computed')
      return new Date().getTime()
    }
  },
  methods: {
    now2: function () {
      console.log('methods')
      return new Date().getTime()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
