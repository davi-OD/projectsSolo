<template>
    <div>
        
        <Body />
        <Telex />

    </div>    
</template>


<script>
import Body from "./Body.vue"
import Telex from "./Telex.vue"

export default {
    name: "Home",
    components: {
        Body,
        Telex
    }
};

</script>


<style scoped>

</style>