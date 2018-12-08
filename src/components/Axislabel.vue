<template>
    <text :x="point.x" :y="point.y">{{stat.label}}</text>
</template>
<script>
var stat = [
    {label:'A',value:100},
    {label:'B',value:100},
    {label:'C',value:100},
    {label:'D',value:100},
    {label:'E',value:100},
    {label:'F',value:100}
]



export default {
  name: "axis-label",
  props: {
    stat: Object,
    index: Number,
    total: Number
  },
  computed: {
    point: function() {
      return valueToPoint(
          +this.stat.value + 10,
          this.index,
          this.total
      )
    }
  }
};
</script>
