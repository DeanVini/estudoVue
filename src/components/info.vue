<template>
    <div>
        <h2>Meu nome é: {{ userObject.name }}</h2>
        <div v-if="frontTechStacks.length > 0">
            <p >Estou usando as tecnologias front-end:</p>
            <ul>
                <li v-for="(tech, index) in frontTechStacks"  :key="index">
                        {{ tech.name }}
                </li>
            </ul>
        </div>

        <div v-if="backEndStacks.length > 0">
            <p>Estou utilizando as tecnologias back-end:</p>
            <ul>
                <li v-for="(tech, index) in backEndStacks" v-bind:key="index">{{ tech.nam }}</li>
            </ul>
        </div>
    </div>
</template>

<script setup>
import { onMounted, ref, watch } from "vue";

const props = defineProps(["userObject"]);

let frontTechStacks = ref(props.userObject.techStacks.filter((tech) => tech.type == 'F'));

let backEndStacks = ref(props.userObject.techStacks.filter((tech) => tech.type == 'B'))

watch(props, (newProps) => {
    frontTechStacks.value = newProps.userObject.techStacks.filter((tech) => tech.type == 'F');
});

watch(props, (backProps) => {
    backEndStacks.value = backProps.userObject.techStacks.filter((tech) => tech.type == 'B');
})


</script>