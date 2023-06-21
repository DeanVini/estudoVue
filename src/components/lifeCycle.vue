<template>
    <p>{{ nome }}</p>
</template>

<script>
    export default{
        name: "lifeCycle",

        data(){
            return{
                nome: 'carregando...'
            }
        },

        created(){
            setTimeout(()=>{
                this.nome = "teste"
            },1000)
        },

        mounted(){
            setTimeout(()=>{
                this.nome = "Dean"
            }, 2000)
        }
    }
    
</script>