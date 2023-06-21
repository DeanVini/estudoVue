<template>
    <div>
        <h2>Esta é uma pessoa: {{ nome }}</h2>
        <info/>

        <a v-bind:href="siteRef" target="_blank">meu site</a>

        <picture/>
    </div>
</template>



<script>
import info from './info.vue';
import picture from './picture.vue';

    export default{
        components:{
            info,
            picture
        },

        nome: "pessoa",

        data(){
            return{
                nome: "Dean",
                siteRef: "https://www.google.com.br/"
            }
        }
    }
</script>