<template>
  <div class="main">
      <a class="card" :href="url" :class="{ 'ismobile':isMobile }">
        <img :src="img" alt="Project Image">
        <p class="text header2">{{title}}</p>    
        <p class="type bodyText">{{type}}</p>
        <p class="year bodyText">{{year}}</p>
      </a>
  </div> 
  <!-- end of main -->
</template>


<script>

export default {
  name: 'ProjectCard',
  components: {

},
data(){
  return{
  }
},
props:{
    url:String,
    img: String,
    title: String,
    type: String,
    year: String,
    isMobile: Boolean
},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../style.scss';

.main{
    margin-left: 10px;
    margin-right: 10px;
    position: relative;
    width: 400px;
    height: 200px;
}

img{
    width: 100%;
    height: 100%;
        transition: transform 0.25s;

}
.text{
  font-size: 45px;
  width: 100%;
  text-align: center;
  pointer-events: none;
  position: absolute;
  top: 25px;
  color: white;
  opacity: 0;
  transition: opacity 0.5s, color 0.5s;
}

a:hover, .ismobile{
  .text{
    color:$primary;
    opacity: 1;
  }

  .type{
    opacity:1;
  }
  .year{
    opacity: 1;
  }

  img{
    transform: scale(1.05);
    filter: brightness(30%);
  }
}

.type{
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
  width: 100%;
  text-align: center;
  pointer-events: none;
  position: absolute;
  bottom: 0px;
  color: white;
  opacity: 0;
  transition: opacity 0.5s, color 0.5s;  
}

.year{
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
  text-align: right;
  pointer-events: none;
  position: absolute;
  right: 10px;
  top: 0px;
  color: white;
  opacity: 0;
  margin: 0;
  padding: 0;
  transition: opacity 0.5s, color 0.5s;    
}

</style>
