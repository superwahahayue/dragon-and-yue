<template>
  <div class="home" id="HomeView">
  <div class="filterBox">
  <span class="text">Ben Is Fall In Love With Master Lu</span>
   </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class HomeView extends Vue {
  [x: string]: any;
  public choose() {
    alert("数据库");
  }
}
</script>
<style>
body{
  background: black;
}
.filterBox{
  margin-top: 50px;
  text-align: center;
  //background: black;
  filter: contrast(30);
}
.text{
  color: #fff;
  margin-top: 100px;
  font-size: 34px;
  font-weight: bold;
  animation: showup 3s forwards;
}
@keyframes showup {
  from{
    letter-spacing: -40px;
    opacity: .6;
    filter:blur(8px);
  }
  to{
    letter-spacing: 5px;
    filter:blur(1px);
    opacity: 1;
  }
  
}

</style>
