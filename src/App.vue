<template>
  <div id="app">
    <div class="nav">
      <navBar class="navBar" :isMobile="isMobile"/>     
    </div>
    <Landing :style="fullHeight" class="landing" :isMobile="isMobile"/>
    <Home :isMobile="isMobile"/>
  </div>
</template>

<script>
import Home from './views/Home.vue';
import Landing from './views/Landing.vue';
import NavBar from './components/NavBar.vue';
export default {
  name: 'app',
  components: {
    Home,
    Landing,
    NavBar
  },
  data(){
    return{
      window: {
        width: 0,
        height: 0
      },
      isMobile: false
    }
  },
  created(){
  // const self = this;
    window.addEventListener('resize', this.handleResize)
    this.handleResize();
  },
  destroyed() {
    window.removeEventListener('resize', this.handleResize)
  },  
  methods:{
    handleResize() {
      this.window.width = window.innerWidth;
      this.window.height = window.innerHeight;
/* eslint-disable no-console */

      if(this.window.width < 600){
        this.isMobile = true;
      }else{
        this.isMobile = false;
      }
    }, 
  },
  computed: {
    fullHeight () {
      return{
        height: this.window.height+'px'
      }
    }
  },
}
</script>

<style lang="scss">
  @import 'style.scss';

  html{
    width: 100%;
  }

  .navBar{
    margin: 0 auto;
    width: 100%;
    z-index: 1000;
    background: $dark;
  }

  .app{
    width: 100%;
    padding: 0;
    margin: 0;
  }

  .landing{
    // height: 1000px;
  }

</style>
