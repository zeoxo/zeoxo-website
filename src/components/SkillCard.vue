<template>
  <div id="card-container">
    <p class="text header2">{{title}}</p>
  </div> 
  <!-- end of main -->
</template>


<script>

export default {
  name: 'SkillCard',
props:{
    title: String,
},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style.scss';
    #card-container{
        border-color: $primary;
        border: 3px solid $primary;
        margin: 4px;
        padding: 4px;    
    .text{
        font-size: 20px;
        cursor: default;
        color: $primary;
    }

}
#card-container:hover{
    border-color: white;
    p{
        color: $light;
    }
}
</style>
