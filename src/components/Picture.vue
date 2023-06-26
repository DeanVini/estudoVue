<template>
    <div>
        <img :src="userObject[count].imgSource" :alt="'nada'" @click="clickImg">
        <info :user-object="userObject[count]"/>
    </div>
</template>

<script setup>
import { ref } from "vue";
import Info from "./info.vue";


const props = defineProps(["userObject"]);


let count = ref(0);

function clickImg(){
    if(count.value > 3){
        count.value = 0;
    }
    else{
        count.value++;
    }

}

</script>

<style scoped>
img{
    transition: all 1s ease;
    border: 20px;
    border-color: blue;
    background-color: blue;
}
</style>