<template>
  <div id="app">
      <svg width="200" height="200">
        <polygragh></polygragh>
      </svg>
      
  </div>
</template>

<script>
import Polygragh from './components/Polygraph.vue'

export default {
  name: 'App',
  components: {
      Polygragh
  },
  created:function () { 
      console.log(this.test())
   }
}
</script>

<style>
body {
    font-family: Helvetica Neue, Arial, sans-serif;
}

polygon {
    fill: #42b983;
    opacity: .75;
}

circle {
    fill: transparent;
    stroke: #999;
}

text {
    font-family: Helvetica Neue, Arial, sans-serif;
    font-size: 10px;
    fill: #666;
}

label {
    display: inline-block;
    margin-left: 10px;
    width: 20px;
}

#raw {
    position: absolute;
    top: 0;
    left: 300px;
}
</style>
