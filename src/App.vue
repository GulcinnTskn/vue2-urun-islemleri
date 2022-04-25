<template>
  <div>
    <app-header></app-header>
    <transition name="fade" mode="out-in">
        <router-view></router-view>
    </transition>
    <br> <br>
  <!-- <app-footer></app-footer> -->
  </div>
</template>


<script>
import Header from "./components/shared/Header.vue";
//import Footer from "./components/shared/Footer.vue";




export default {
  components: {
    appHeader: Header,
  //  appFooter: Footer,


  },
  created() {
    this.$store.dispatch("getTradeResult")
    this.$store.dispatch("initApp")
  }
};
</script>


<style>
body{
  background-color: rgb(232, 219, 245);
}
.fade-enter{
  opacity: 0;
}
.fade-enter-active{
  transition : opacity 0.3s ease-out;

}
.fade-leave{}
.fade-leave-active{
  transition: opacity 0.3s ease-out;
  opacity: 0;
}

</style>
