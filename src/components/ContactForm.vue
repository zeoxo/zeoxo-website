<template>
  <div class="main">
    <form action="" style="text-align: left;">
        <input class="bodyText" type="text" placeHolder="name"> <br>
        <input class="bodyText"  type="email" placeHolder="email">  <br> 
        <input class="bodyText"  type="text" placeHolder="subject">  <br> 
        <textarea class="bodyText"  name="message" rows="1" cols="25" placeholder="Message"></textarea>   <br>
        <input class="header1 submit" type="submit">
    </form>
  </div> 
  <!-- end of main -->
</template>


<script>

export default {
  name: 'ContactForm',
  components: {

},
data(){
  return{
  }
},
props:{
},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../style.scss';

    form{
        input, textArea{
            color: $dark;
            margin: 30px;
            font-size: 150%;
            outline: none;
            border: none;
            background: $light;
            border-bottom: 1px solid;
            border-color: $primary;
        }

        .submit{

            border: 2px solid;
            border-color: $primary;
            color: $dark;
            font-size: 30px;
            padding: 10px;
            &:hover{
                color: white;
                background: $primary;
            }
        }
    }

</style>
