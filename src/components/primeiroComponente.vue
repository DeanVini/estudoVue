<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é {{ nome }} e trabalho na {{ workAt }}</p>
    </div>
</template>

<script>

    export default{
        name: 'primeiroComponente',
        data(){
            return{
                nome: "Dean",
                workAt: "PGM"
            }
        }
    }</script>