
<template>
  <div id="app">
    <leftNav />
    <div class="main">
      <router-view ></router-view>
      <!-- <transition name="fade"></transition> -->
    </div>
  

  </div>
</template>

<script>
import leftNav from '@/components/common/leftNav'
export default {
  name: "App",
  components:{
    leftNav
  }
};
</script>

<style>
.fade-enter {
  opacity:0;
}
.fade-leave{
  opacity:1;
}
.fade-enter-active{
  transition:opacity .5s;
}
.fade-leave-active{
  opacity:0;
  transition:opacity .5s;
}
.main{
  float: left;
  width: 95%;
  background-color: #eff2f7;
  height: 100%;
  overflow: hidden;

}
</style>
