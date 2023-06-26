<template>
<div>
    <h2>Meu form</h2>
    <form @submit="submitForm($event)">
        <input type="text" v-model="nome">
        <input type="text" v-model="email">
        <input type="submit">
    </form>
</div>    
</template>

<script setup>

let nome= '';
let email = '';

function submitForm(e){
    e.preventDefault();
    console.log("meu nome é:",this.nome);
    console.log("meu email é:",this.email);
    
}
// export default{
//     name: 'Comment',

//     data(){
//         return{
//             nome: '',
//             email: ''
//         }
//     },

//     methods:{
//         submitForm(e){
//             console.log(e);
//             e.preventDefault();
//             console.log("meu nome é:",this.nome);
//             console.log("meu email é:",this.email);

//         }
//     }
// }
</script>

<style scoped>

</style>