<template>
    <div class="television">
        <div class="div" v-if="tele" id="grey">
        </div>
        <div class="div" v-else id="black">
        </div>
        <button class="btn btn-primary" type="submit" v-on:click="teleMethod">Power</button> 
    </div>
</template>

<script>
    export default {
        name:'Tele',
        data: function(){
            return{
                tele:true
            }
        },

        methods:{
            teleMethod: function(){
                this.tele = !this.tele 
            }
        }
    }
    // :src="require(`@/assets/<'fileName'>`) 
</script>

<style scoped>

    .Tele-switch{
        margin:8% auto;
        width:710px;
        background-color:rgb(70, 63, 63);
        border:5px solid black;
        height:500px;
    }
    .div{
        width:350px;
        height:350px;
    }
  
    #grey{
        background-image:url('../assets/On.gif'); 
        width:700px;
    }
    #black{
        background-color:black;
        width:700px;
    }
#black{
        background-color:black;
        width:700px;
    }

    .btn{
        width:80px;
        height:80px;
        border-radius: 50%;
        color:white;
        background-color: rgb(26, 155, 37) !important;
        margin-top:15px;
    }
    .btn:focus{
        outline:0 !important;
        box-shadow:none !important;
        border-color:gray;
    }
    .btn:hover{
        color:white;
        background-color:red !important;
    }
</style>
