<template>
  <h1>The Journey</h1>
  <div><Image /></div>
  <div><TheCalc /></div>
  <div><WalkLog /></div>
</template>

<script>
// @ is an alias to /src
//import comp from "@/components/comp.vue";
import Image from "@/components/AdventureImage.vue";
import TheCalc from "@/components/WalkCalc.vue";
import WalkLog from "@/components/WalkLog.vue";

export default {
  name: "Main",
  components: {
    Image,
    TheCalc,
    WalkLog
    //    comp,
  }
};
</script>
