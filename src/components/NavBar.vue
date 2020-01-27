<template>
  <div class="main">
    <a href="">  
        <img class="logo" src="../assets/svg/logo.svg">
    </a>
  
    <div class="right">

      <!-- if on desktop -->
        <div class="linksDesktop" v-if="!isMobile" :class="{ 'linksMobile':isMobile }">
            <a @click="scrollToAbout">About</a>
            <a @click="scrollToSkills">Skills</a>
            <a @click="scrollToProjects">Projects</a>
            <div class="vl"></div>
            <a @click="scrollToContact">Contact</a>
        </div>

      <div class="linksMobile" v-if="isMobile">
        
      </div>
    </div>

  </div> 
  <!-- end of main -->
</template>


<script>
var scrollToElement = require('scroll-to-element');
export default {
  name: 'NavBar',
  components: {

},
props:{
  isMobile: Boolean
},
data(){
  return{
  }
},  
  methods:{
    scrollToAbout(){
      scrollToElement('#about');
    },
    scrollToSkills(){
      scrollToElement('#skills');
    },
    scrollToProjects(){
      scrollToElement('#projects');
    },
    scrollToContact(){
      scrollToElement('#contact');
    }

  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../style.scss';

    .main{
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        display: flex;
        justify-content: space-between;
    }

  .right{
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-right:1%;
    flex-wrap: nowrap;
    padding: 5px;
    align-items: flex-start;
  }

  .linksDesktop{
    display: flex;
    flex-direction: row;
    // flex-wrap: nowrap;
    align-items: center;
    a{
      cursor: pointer;
      white-space:nowrap;
      padding-left: 15px;
      padding-right: 15px;
      text-align: center;
      font-size: 100%;
      font-family: "optician-sans";
      color: white;
      text-decoration: none;
    }

      a:hover{
          color:$primary;
      }
  }
  .linksMobile{
    display: flex;
    flex-direction: column;
    align-items: left;
    a{
      cursor: pointer;
      white-space:nowrap;
      padding-left: 15px;
      text-align: left;
      font-size: 100%;
      font-family: "optician-sans";
      padding-bottom: 10px;
      color: white;
      text-decoration: none;
    }

      a:hover{
          color:$primary;
      }
  }


  .logo{
      height: 40px;
      margin-left: 2%;

      &:hover{
        transition: transform 0.5s;

      }
  }

</style>
