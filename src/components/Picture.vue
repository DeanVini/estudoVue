<template>
    <img :src="pic" :alt="comment" @click="clickImg">
</template>

<script>
export default {
    name: 'Picture',
    data() {
        return {
            pic: 'https://avatars.githubusercontent.com/u/85954641?v=4',
            comment: 'gaybriel',
            count: 1

        }
    },
    methods:{
        clickImg(){
            this.count ++;
            if(this.count == 2){
                this.pic = "https://avatars.githubusercontent.com/u/81484737?v=4"

            }

            if(this.count == 3){
                this.pic = "https://avatars.githubusercontent.com/u/42882594?v=4"

            }

            if(this.count == 3){
                this.pic = "https://avatars.githubusercontent.com/u/42882594?v=4"

            }

            
        }
    }
}
</script>

<style>

</style>