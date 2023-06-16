<template>
    <main>
        <div class="main-part">
            <AppCards class="card"/>
        </div>
    </main>
</template>
<script>
import AppCard from './cards/AppCard.vue'
export default {
    name: 'AppMain',
    components:{
        AppCard
    },
    data(){
        return{

        }
    }
}
</script>

<style lang="scss" scoped>
    main{
        background-color: black;
        color: white;
        height: 130px;
        margin: 0 auto;
    }
    .main-part{
        width: 70%;
        margin: 0 auto;
    }
    .card{
        width: calc(100% / 6);
    }
</style>