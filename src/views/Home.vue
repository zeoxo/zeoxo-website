<template>
  <div class="main">
    <!-- ABOUT -->
    <div class="aboutContainer" id="about">
    <div class="about" style="padding-top: 70px;">
      <p class="titleText primary">&lt; About &gt;</p>
      <div class="aboutMe" :class="{ 'aboutMe-mobile':isMobile }">
        <img src="https://media.licdn.com/dms/image/C4E03AQFSRVHnLJZ1Cw/profile-displayphoto-shrink_200_200/0?e=1580342400&v=beta&t=985W4dZuXHvMttXCAVYh6lBh_8Yx8kHCnqkhiMZ0580" alt="me">
        <p class="bodyText med">My name is Dylan Dougherty, Known online as zeoxo, and I love to learn. Throughout my life I have dedicated myself to learning and mastering new skills. 
          Whether that be in the world of technology, the art of ceramics, or even snowboarding. I am always looking for the next thing to pick up and try. I am self-taught in the areas of game development and graphic design,
          while also having formal training in the form of a Bachelor's of science in Information Technology and a Minor in Web Developement from Kutztown University of Pennsylvania. 
        </p> 
  
      </div>
    </div>
      <div class="titleText primary" id="skills" style="padding-top: 50px;">&lt; Skills &gt;</div>
      <div class="skills" style= "width: 65%; margin: 0 auto;">
        <div class="code" style="text-align: left;">
          <p class="header1 dark">Coding</p>
          <p class="bodyText med">I have exensive experience with many languages including javscript, c#, c++, Java, and Python. For the last few years I have
            dedicated most of my learning to C# and the Unity Game engine.
          </p>
        </div>  
        <div class="art" style="text-align: left;">
          <p class="header1 dark">Art</p>
          <p class="bodyText med">I am self trained in many graphic design applications such as Afinity Designer and Afinity Photo. These are comparable 
            to both Illustrator and Photoshop respectively. </p>
        </div>  
      </div>  
    </div>


    <!-- PROJECTS -->
    <div class="projects" id="projects">
      <p class="titleText primary " style="padding-top: 50px; padding-bottom: 100px;">&lt; Projects &gt;</p>
      <p class="header2 light">Software</p>
      <div class="projectCards">
        <ProjectCard class="card" url="https://google.com" img="https://i.ibb.co/nPL0zM8/flyta.png" title="FLYTA" type="mobile game" year="TBD"  :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://google.com" img="https://compote.slate.com/images/697b023b-64a5-49a0-8059-27b963453fb1.gif" title="Social Study" type="web app" year="2019" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://google.com" img="https://i.stack.imgur.com/XW25s.jpg" title="Coffé" type="mobile app" year ="2018" :isMobile="isMobile"/>   
        <ProjectCard class="card" url="https://zeoxo.itch.io/paper-or-plastic" img="https://img.itch.zone/aW1hZ2UvMTA0NDgxLzQ4NTYxNy5wbmc=/347x500/VylktR.png" title="Paper or Plastic" type="iOS game" year="2016" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.itch.io/the-ninth-circle" img="https://img.itch.zone/aW1hZ2UvMTA0NDY2LzQ4NTU2Mi5wbmc=/original/yP4c7Q.png" title="Ninth Circle" type="jam game" year="2016" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.itch.io/slap-fight" img="https://img.itch.zone/aW1hZ2UvMTQ2OTA0LzY3Mzg0Ny5wbmc=/original/QM%2B8vu.png" title="slap Fight!" type="jam game" year="2017" :isMobile="isMobile"/>
      </div>
      <div class="art">
        <p class="header2 light" style="padding-bottom: 30px;">Art</p>
        <div class="artContainer">
          <img class="artImage" src="../assets/images/projects/art/computer.gif" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/DestinyGhost.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/instArt_house.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/instArt_Skeleton.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/Lettuce_2.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/SodaSpin.gif" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/LeviathanAxe.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/plasmaCutter_Final.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/Potion_color.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/recordPlayer.gif" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/SrugglesLogo_Ocean.png" alt="artImage">
          <img class="artImage" src="../assets/images/projects/art/Sword.png" alt="artImage">
        </div>
      </div>
    </div>
    
    <!-- CONTACT  -->
    <p class="titleText primary contact-container" id="contact">&lt; Contact &gt;</p>
    <div class="contact">
      <div class="form">
        <ContactForm/>
      </div>
      <div class="icons">
        <div class="email">
          <img src="../assets/svg/email.svg" alt="email" class="emailSVG">
          <p class="header1 dark" style="padding-top: 20%;">Email</p>
          <a href="mailto: dyldougherty@gmail.com">
            <p class="bodyText primary">dyldougherty@gmail.com</p>
          </a>
        </div>
        <div class="location">
          <img src="../assets/svg/location.svg" alt="location" class="locationSVG">
          <p class="header1 dark" style="padding-top: 20%;">Location</p>
          <a href="https://www.google.com/maps?q=philadelphia+pennsylvania&rlz=1C1GCEA_enUS851US851&um=1&ie=UTF-8&sa=X&ved=2ahUKEwjbwJe6goXmAhXpY98KHZc-B2AQ_AUoAXoECBgQAw">
            <p class="bodyText primary">Phildadelphia, Pennsylvania</p>
          </a>
        </div>
      </div>

    </div>

  <!-- <p>Icons from https://icons8.com/</p> -->
  <div class="footer">
    <div id="content">
      <div class="bodyText" style="vertical-align:middle;">
        © Copyright 
        <div class="titleText primary" style="display:inline; font-size: 25px;">zeoxo</div>  
        2019
      </div>
      <div class="socialLinks">
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
      </div>
    </div>
  </div> <!-- end of main -->
</template>

<script>
import ProjectCard from "../components/ProjectCard.vue";
import ContactForm from "../components/ContactForm.vue"
var scrollToElement = require('scroll-to-element');
export default {
  name: 'Home',
  data(){
    return{
      subTextIndex: 0,
    }
  },
  props:{
    isMobile: Boolean
  },
  components: {
    ProjectCard,
    ContactForm
  },
  mounted(){
    setInterval(() => {
      this.incrementsubText();
    }, 1500);
  },
  methods:{
    incrementsubText(){
      if(this.subTextIndex < 2){
        this.subTextIndex += 1;
      }else{
        this.subTextIndex = 0;
      }
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
      margin: 0 auto;
      text-align: center;
      margin-top: 2%; 
    }
    .about{
      background:white;
      width: 100%;
      margin: 0 auto;

      .aboutMe{
          display: flex;
          margin: 0 auto;
          flex-wrap: wrap;
          width: 50%;
          justify-content: center;

        p{
            text-align: left;
            width: 100%;

          }

        img{
          border-radius: 100%;
          width: 100px;
          height: 100px;
          padding: 0px;
          margin-top: 30px;
          filter: grayscale(100%);
        }
      }
      .aboutMe-mobile {
                display: flex;
                margin: 0 auto;
                flex-wrap: wrap;
                width: 100%;
                justify-content: center;

              p{
                  text-align: left;
                  width: 90%;

                }

              img{
                border-radius: 100%;
                width: 100px;
                height: 100px;
                margin-right: 30px;
                margin-top: 30px;
                filter: grayscale(100%);
              }
            }



    }

  .projectCards{
    align-content: flex-start;
    align-items: flex-start;
    margin: 0 auto;
    width: 80%;
    padding: 0;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    padding-bottom: 100px;
  }

  .header1{
    padding-top: 100px;
  }

  .card{
    margin-top: 25px;
  }

.aboutContainer{
  background: $light;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.projects{
  background: $dark;
}

.artContainer{
  width: 80%;
  margin: 0 auto;
  .artImage{
    width: 300px;
    height: 300px;
  }
}

.contact-container{
  background: $light;
}

.contact{
  display: flex;
  width: 100%;
  justify-content: center;
  flex-wrap: wrap;
  background-color: $light;
  .email, .location{
    color: $light;
    margin: 30px;
    a{
      text-decoration: none;
    }
  }
  
  .emailSVG, .locationSVG{
    width: 40%;
  }
}


.footer{
  padding-top: 200px;
  padding-bottom: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 0 auto;

  background: $dark;

  #content{
    color: $medium-light;
    font-size: 11px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 75%;
    a{
      padding: 10px;
    }
    img{
      padding-top: 0px;
      height: 25px;
    }
  }
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
