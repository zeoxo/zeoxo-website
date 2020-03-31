<template>
  <div class="main">
    <!-- ABOUT -->
    <div class="aboutContainer" id="about">
    <div class="about" style="padding-top: 70px;">
      <p class="titleText primary">&lt; About &gt;</p>
      <div class="aboutMe" :class="{ 'aboutMe-mobile':isMobile }">
        <p class="bodyText dark">
          My name is Dylan Dougherty, better known online as zeoxo. I am a passionate web and game developer who loves creating interative experiences for all to enjoy. Scroll down to take a look at some of my past projects, and what im currently working on!
        </p> 
  
      </div>
    </div>
      <div class="titleText primary" id="skills" style="padding-top: 120px;">&lt; Skills / Experience &gt;</div>
      <div class="skills" style= "width: 65%; margin: 0 auto;">
        <div class="education" style="text-align: left;">
          <p class="header1 primary">Education</p>
          <hr style="margin-bottom: 30px;">
            <a class="header3" target="_blank" href="https://www.kutztown.edu/"> Kutztown University</a>
            <ul class="list light">
              <li>Major: B.S. Information Technology</li>
              <li>Minor: Web Development</li>
              <li>Member of the National Honors Society For Leadership and Success</li>
              <li>Dean’s list Spring 2019</li>
              <li>Senior Project adopted by univerity for internal use</li>
            </ul>
        </div>
        <div class="code" style="text-align: left;">
          <p class="header1 primary">Dev</p>
          <hr>
          <p class="bodyText light">
            Development is one of my biggest passions. Throughout both my academic career at <a target="_blank" href="https://www.kutztown.edu/"> Kutztown University</a>, 
            and my own personal endevours, I have dived into a variety of languages and tools.
          </p>
          <div class="skillCards">
            <SkillCard class="skillCard" title="HTML"/>
            <SkillCard class="skillCard" title="CSS"/>
            <SkillCard class="skillCard" title="JavaScript"/>
            <SkillCard class="skillCard" title="C++"/>
            <SkillCard class="skillCard" title="C#"/>
            <SkillCard class="skillCard" title="React"/>
            <SkillCard class="skillCard" title="React Native"/>
            <SkillCard class="skillCard" title="Vue"/>
            <SkillCard class="skillCard" title="Unity"/>
            <SkillCard class="skillCard" title="Game Maker"/>
            <SkillCard class="skillCard" title="Python"/>
            <SkillCard class="skillCard" title="Java"/>
            <SkillCard class="skillCard" title="Ionic"/>
            <SkillCard class="skillCard" title="VueX"/>
            <SkillCard class="skillCard" title="JSON"/>
            <SkillCard class="skillCard" title="Firebase"/>
            <SkillCard class="skillCard" title="NativeScript"/>
            <SkillCard class="skillCard" title="Git"/>
            <SkillCard class="skillCard" title="NPM"/>
            <SkillCard class="skillCard" title="Database Design"/>
            <SkillCard class="skillCard" title="PHP"/>
            <SkillCard class="skillCard" title="SQL"/>
            <SkillCard class="skillCard" title="WEB VR"/>
            <SkillCard class="skillCard" title="SQL"/>
            <SkillCard class="skillCard" title="SQL"/>
            <SkillCard class="skillCard" title="Processing"/>
            <SkillCard class="skillCard" title="Computer Vision"/>
            <SkillCard class="skillCard" title="VR"/>
            <SkillCard class="skillCard" title="A-Frame"/>
            <SkillCard class="skillCard" title="Express"/>
            <SkillCard class="skillCard" title="Node"/>
            <SkillCard class="skillCard" title="XCode"/> 
          </div>
        </div>  
        <div class="Design" style="text-align: left;">
          <p class="header1 primary">Design</p>
          <hr>
          <p class="bodyText light">I am self trained in graphic design and web design practices. I use my skills to develop small art pieces, logos, and websites. 
            I also have experience with ceramic art and specialize in wheel thrown pieces.
          </p>
          <div class="skillCards">
            <SkillCard class="skillCard" title="Afinity Photo"/> 
            <SkillCard class="skillCard" title="Afinity Designer"/>
            <SkillCard class="skillCard" title="web design"/>
            <SkillCard class="skillCard" title="Figma"/> 
            <SkillCard class="skillCard" title="Logo Design"/> 
            <SkillCard class="skillCard" title="UI Design"/>
          </div>
        </div>  
      </div>  
    </div>


    <!-- PROJECTS -->
    <div class="projects" id="projects">
      <p class="titleText primary " style="padding-top: 50px; padding-bottom: 100px;">&lt; Projects &gt;</p>
      <p class="header2 light">Software</p>
      <div class="projectCards">
        <ProjectCard class="card" url="https://zeoxo.com" img="https://i.ibb.co/LdfQDDZ/coastal.gif" title="COASTAL" type="WIP Game" year="TBD"  :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://flytagame.com" img="https://i.ibb.co/fMv4y0J/flyta.gif" title="FLYTA" type="mobile game" year="2019"  :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://socialstudy.app/" img="https://i.ibb.co/MkCzmMH/social-Study.gif" title="Social Study" type="web app" year="2019" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.itch.io/slap-fight" img="https://i.ibb.co/LCtrGcY/slap-Fight.gif" title="slap Fight!" type="jam game" year="2017" :isMobile="isMobile"/>        
        <ProjectCard class="card" url="https://zeoxo.itch.io/the-ninth-circle" img="https://i.ibb.co/W3v2yf8/ninth-Circle.gif" title="Ninth Circle" type="jam game" year="2016" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.itch.io/paper-or-plastic" img="https://i.ibb.co/Jyb00yQ/paperorplastic.gif" title="Paper or Plastic" type="iOS game" year="2016" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.github.io/Table-Games/" img="https://zeoxo.github.io/Table-Games/images/table3.png" title="Table Games" type="computer vision experiment" year="2019" :isMobile="isMobile"/>
        <ProjectCard class="card" url="https://zeoxo.github.io/Another-Place/" img="https://i.ibb.co/JkQg4F4/Another-Place.png" title="Another Place" type="Web AR Experiment" year="2019" :isMobile="isMobile"/>

      </div>

        <p class="header2 light" style="padding-bottom: 30px;  padding-top: 80px;">Art</p>
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
    
    <!-- CONTACT  -->
    <div class="contact" id="contact">
      <p class="titleText primary " style="width: 100%; padding-top: 60px; padding-bottom:50px;">&lt; Contact &gt;</p>
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
import SkillCard from '../components/SkillCard'
// import ContactForm from "../components/ContactForm.vue"
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
    SkillCard,
    // ContactForm
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
      background:$light;
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
  background: $dark;
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

.skillCards{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-start;
  align-content: flex-start;
}

</style>
