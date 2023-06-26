<template>
    <div>
        <button @click="firstEv(txt1, $event), secEV(txt2, $event)">Ativar multiplos eventos</button>
        <p>{{ multiple_event }}</p>
    </div>
</template>

<script>
export default {
    name: 'MultipleEvets',

    data(){
        return{
            multiple_event: '',
            txt1: 'Primeiro evento',
            txt2: 'Segundo evento'
        }
    },

    methods:{
        firstEv(txt,e){
            this.multiple_event = txt;
        },

        secEV(txt,e){
            setInterval(()=>{
                this.multiple_event = txt;
            }, 1000)
        }
    }
}


</script>

<style scoped>

</style>