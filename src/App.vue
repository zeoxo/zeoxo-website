<template>
  <div id="app">
    <div class="bg"></div>
    <div class="nav">
      <navBar class="navBar"/>     
    </div>
    <Landing class="landing"/>
  </div>
</template>

<script>
import Landing from './views/Landing.vue';
import NavBar from './components/NavBar.vue';
export default {
  name: 'app',
  components: {
    Landing,
    NavBar
  },
  data(){
    return{
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
    margin-top: 30px;
    width: 75%;
  }
  .bg{
    position: fixed;
    width: 100%;
    height: 100%;
    z-index: -100;
    margin:0 auto;
    top:0;
    left: 0;
    background-image: url("./assets/images/background.png");
    background-size: 75%;
    opacity: .75;
  }

  .app{
    width: 100%;
    padding: 0;
    margin: 0;
  }

</style>
