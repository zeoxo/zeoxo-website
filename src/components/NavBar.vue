<template>
  <div class="main">
    <a href="">  
        <img class="logo" src="../assets/svg/logo.svg">
    </a>
  
    <div class="right">

      <!-- if on desktop -->
        <div class="linksDesktop" v-if="window.width > 600">
            <a href="">About</a>
            <a href="">Projects</a>
            <a href="">Links</a>
            <div class="vl"></div>
            <a href="">Contact</a>
        </div>

        <!-- mobile -->
        <div class="linksMobile" v-if="window.width < 600">
            <a href="">About</a>
            <a href="">Projects</a>
            <a href="">Links</a>
            <a href="">Contact</a>
        </div>
    </div>

  </div> 
  <!-- end of main -->
</template>


<script>

export default {
  name: 'NavBar',
  components: {

},
data(){
  return{
    window:{
      width: 0,
      height: 0
    }
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
    },
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../style.scss';

    .main{
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
