<template>
    <div>
        <Picture :userObject="data"/>

        <a :href="''" target="_blank">meu site</a>

    </div>
</template>



<script setup>
import Picture from "./Picture.vue";
import { data } from '../utils/data.js';
import { onMounted, ref } from "vue";


</script>