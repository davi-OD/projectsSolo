<!-- <div class="container">
    <h1 v-if="toggle">on</h1>
    <h1 v-else>off</h1>

    <frame-row> 
    <frame-col>  
    <button class="btn btn-primary" v-on:click="toggleMethod">Toggle</button>
    </frame-col>
    </frame-row>
  </div> -->
<template>
 
  <img src="require('@/assets/tv.png')">
  <img src="tv.png">


</template>

<script>
import image from "assets/tv.png"
export default {
name:"Body",
data: function () {
            return {
                toggle:true,
                image: image
            }
            
        },
        methods:{
        toggleMethod:function(){
            this.toggle=!this.toggle
        }
    }

    
  
}
</script>



<style scoped>
div {
 align-content: center;
  background-color: lightgrey;
  width: 500px;
  height: 500px;
  border: 15px solid rgb(11, 12, 11);
  padding: 50px;
  margin: center;
}
button{
    float: right;
    
}
</style>
