<template>
    <div>
        <div>
            <h1 v-if="state">Bulb is On</h1>
            <h1 v-else>Bulb is Off</h1>
            <button class="btn btn-primary" v-on:click="changeState">
                <span v-if="state">Turn Off</span>
                <span v-else>Turn On</span>
            </button>
            <a v-bind:href="googleLink">Google</a>

        </div>
    </div>
</template>


<script>
export default {
    name: "NwBody",

    data: function(){
        return {
            state: false,
           googleLink: "www.google.com",
           television: {
                
           }
        }
    },

    methods: {
        changeState:function(){
            this.state = !this.state
        }
    }
    
};
</script>

<style scoped>
/*
    Props
    Slots

    Vue Router (Vue-Router-next lib)
    
    State Management [Vuez lib]
    Building Components (Vuetify lib)
    VENoN Stack
    Nuxjs
    REST APIs / GraphQL

    Event: -Click, Scroll
    Event Listeners: - onClick, onScroll
    Event Handlers: -handleClick(), handleScroll()
*/ 

</style>

