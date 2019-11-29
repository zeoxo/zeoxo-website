<template>
  <div class="main">
    <div class="intro">

      <p class="header2 med-light" style="padding-top: 70px;">{{hello}}</p>
      <div style="vertical-align:middle; padding-top: 10px;">
      <div class="name">
        <p class="header1 light" style="display: inline;  font-size: 650%;">I am </p>
        <p class="titleText primary" style="display:inline; font-size: 500%;">zeoxo</p>  
      </div>
      </div>
      <div class="bodyText light" style="padding: 0; margin: 10px;">

        <div class="subTitle">
          <div v-if="subTextIndex == 0">
            Game 
            <p class="bodyText primary" style="display: inline;">Developer</p>
          </div>
          <div v-if="subTextIndex == 1">
            Web 
            <p class="bodyText primary" style="display: inline;">Developer</p>
          </div>        
          <div v-if="subTextIndex == 2">
            Graphic
            <p class="bodyText primary" style="display: inline;">Designer</p>
          </div>         
        </div>

      
      
      
      </div>
      <div class="socialLinks" style="padding-top: 60px;">
          <a href="https://twitter.com/zeoxo">
            <img src="../assets/svg/twitter.svg" alt="twitter">
          </a>
          <a href="https://www.instagram.com/zeoxo/">
            <img src="../assets/svg/insta.svg" alt="instagram">
          </a>
          <a href="https://dribbble.com/zeoxo">
            <img src="../assets/svg/dribble.svg" alt="dribble">
          </a>
          <a href="https://zeoxo.itch.io/">
            <img src="../assets/svg/itch.svg" alt="itch">
          </a>
        </div>
        <button @click="scrollToAbout"> &#9660; Learn More  &#9660;</button>
    </div>
  </div> <!-- end of main -->
</template>

<script>
var scrollToElement = require('scroll-to-element');
export default {
  name: 'Landing',
  data(){
    return{
      subTextIndex: 0,
      hello: ' '
    }
  },
  props:{
    isMobile: Boolean
  },
  components: {
  },
  mounted(){
    setInterval(() => {
      this.incrementsubText();
    }, 1500);
    
    setTimeout(() => { this.incrementTitle('h'); }, 100);
    setTimeout(() => { this.incrementTitle('e'); }, 200);
    setTimeout(() => { this.incrementTitle('l'); }, 300);
    setTimeout(() => { this.incrementTitle('l'); }, 400);
    setTimeout(() => { this.incrementTitle('o'); }, 500);

    setTimeout(() => { this.incrementTitle(' w'); }, 600);
    setTimeout(() => { this.incrementTitle('o'); }, 700);
    setTimeout(() => { this.incrementTitle('r'); }, 800);
    setTimeout(() => { this.incrementTitle('l'); }, 900);
    setTimeout(() => { this.incrementTitle('d'); }, 1000);
    setTimeout(() => { this.incrementTitle(';'); }, 1100);

  },
  methods:{
    incrementsubText(){
      if(this.subTextIndex < 2){
        this.subTextIndex += 1;
      }else{
        this.subTextIndex = 0;
      }
    }, 
    incrementTitle(char){
      this.hello += char;
    }, 
    scrollToAbout(){
      scrollToElement('#about');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../style.scss';

.main{
  display: flex;
  height : 100%;
  width: 100%;
  justify-content: center;
  text-align: center;
  
  button{
    outline: none;
    width: 200px;
    height: 80px;
    text-align: center;
    margin: 0 auto;
    background: transparent;
    color: White;
    border-width: 4px;  
    border-style: solid;
    border-color: $primary;
    font-size: 20px;
    font-family: 'Poppins', sans-serif;
    margin-bottom: 150px;
    margin-top: 70px;

    &:hover{
      color: $dark;
      background: $primary;
    }
  }
}

.name{
  opacity: 0;
  animation: fadeIn 2s;
  animation-delay: 1.2s;
  animation-fill-mode: forwards;
}
.subTitle{
  opacity: 0;
  animation: fadeIn 2s;
  animation-delay: 1.5s;
  animation-fill-mode: forwards; 
}

button, .socialLinks{
  opacity: 0;
  animation: fadeIn 2s;
  animation-delay: 2s;
  animation-fill-mode: forwards;   
}

  @keyframes fadeIn {
    to{
      opacity: 1;
    }
  }

.intro{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
}
.socialLinks{
  margin: 0 auto;
  width: 50%;
  padding-top: 20px;
  img{
    height: 50px;
    padding: 8px;
    transition: transform 0.2s;
  }
  img:hover{
    transform: scale(1.5);
    fill: $primary;
  }
}

</style>
