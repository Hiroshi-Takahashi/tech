<template>
  <svg xmlns="http://www.w3.org/2000/svg" :width="width" :height="height" style="background-color:black">
    <MyPolyLine points="10 200 126 100 242" stroke="#333" strokeWidth="2"></MyPolyLine>
  </svg>
</template>

<script>
import PolyLine from '@/components/parts/PolyLine'

export default {
  name: 'LineChart',
  components: {
    'MyPolyLine': PolyLine
  },
  props: {
    width: Number,
    height: Number,
    fill: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
