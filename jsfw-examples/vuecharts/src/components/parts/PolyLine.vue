<template>
<!--
  <polyline :points="points" fill="none" :stroke="stroke" :stroke-width="strokeWitdh"></polyline>
-->
  <polyline points="10 200 126 100 242 150 358 50 474 300 590 250" fill="none"  stroke="#00FF00" stroke-width="1"></polyline>
</template>

<script>
export default {
  name: 'PolyLine',
  props: {
    points: String,
    stroke: String,
    strokeWidth: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
