<template>
  <div>
      <shape-shifter :content="content" :width="width" :height="height" :fontSize="fontSize"></shape-shifter>
  </div>
</template>

<script>
import shapeShifter from "./components/ShapeShifter.vue"

export default {
  components: { shapeShifter },
  data () {
    return {
      content: "hello|你好|shape-shifter|#countdown 3|",
      width: 1500,
      height: 600,
      fontSize: 150
    }
  }
}
</script>
