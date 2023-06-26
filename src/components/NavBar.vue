<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Perfil</a></li>
    </ul>    
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
    
};

li{
    margin-right: 100px;
}

a{
    color: #ddd;
    text-decoration: none;
    transition: .5s;
}

a:hover{
    color:turquoise
}

</style>