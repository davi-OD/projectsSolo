<template>
    <div class="container">
        <div class="row"  style="text-align:left">
            <div class="col-4">
                <h3>Student Registration Form</h3>
                <hr>
                <h5>{{studentName}}</h5>

                <div class="input-group mb-3">
                <input v-model="studentName" type="text" class="form-control" placeholder="Student Name" aria-label="Recipient's username" aria-describedby="button-addon2">
                <button v-on:click="registerStudent" class="btn btn-primary" type="button" id="button-addon2">Register</button>
                </div>

            </div>
            <div class="col-8">
                <h3>Student Registration List</h3>
                <ol class="list-group list-group-numbered">
                    <li class="list-group-item" v-for="student in students" v-bind:key="student">{{student}}</li>
                </ol>
            </div>
        </div>
    </div>    
</template>

<script>
    export default {
        data(){return {
            students:[],
            studentName:""
        }},
        methods:{
            registerStudent:function(){
                this.students.push(this.studentName);
            }
        },
        components:{},
        name:"Body",
    }

    /*
        Props
        Slots 

        Routing (Vue-Router-next lib)
        State Management [Vuex lib]
        Building Components (Vuetify lib)
        VENoM Stack
        Nuxtjs
        REST APIs / GraphQL
    */ 

</script>

<style scoped></style>
