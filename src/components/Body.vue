<template>
    <div id="elem">
        <div class="container">   
        <h1 v-if="toogle">On</h1> 
        <h1 v-else>Off</h1> 

        <frame-row>
        <frame-row>
        <button class="btn btn-primary" v-on:click="toggleMethod">Toggle</button>
        </frame-row>
        </frame-row>
        </div> 
    </div>    
</template>

<script>
export default {
    name: "Body",
     data: function(){
        return {
            toggle: true
            }
    },
    methods: {
        toggleMethod:function(){
            this.toggle = !this.toggle
        }
    }
    
}
</script>

<style scoped>

</style>