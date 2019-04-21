<template>
  <div class="Home-head">
    <!-- <img src="./1.jpg" alt> -->
    <canvas id="tutorial" width="150" height="150"></canvas>
  </div>
</template>
<script>
import { constants } from "crypto";
var ctx = document.getElementById("tutorial").getContext('2d');
export default {
  created() {
  console.log(ctx)
  },
  data() {
    return {
      name: "one"
    };
  }
};
</script>
<style lang="scss" scoped>
.Home-head {
  width: 100%;
  height: 250px;
  font-size: 50px;
  border: 1px solid red;
  overflow: hidden;
  img {
    width: 100%;
  }
  //   transform: rotateX(80deg);
  animation: mymove 2s infinite;
  transform-origin: 100% 50px;
}
.Home-head:before {
  // content: "";
  top: -20px;
  left: 20px;
  width: 100px;
  height: 100px;
  border: 1px solid red;
}
@keyframes mymove {
  0% {
    transform: rotateX(0deg);
  }
  100% {
    transform: rotateX(80deg);
  }
}
</style>

