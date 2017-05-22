<template>
  <div>
      <shape-shifter :content="content" :width="width" :height="height"></shape-shifter>
  </div>
</template>

<script>
import shapeShifter from "./components/ShapeShifter.vue"

export default {
  components: { shapeShifter },
  data () {
    return {
      content: "hello|shape-shifter|#countdown 3|",
      width: 1200,
      height: 600
    }
  }
}
</script>
