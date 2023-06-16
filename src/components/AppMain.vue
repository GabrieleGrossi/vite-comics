<template>
    <main>
        <div class="main-part">
            <AppCards class="card"/>
        </div>
    </main>
</template>
<script>
import AppCards from './AppCards.vue';
export default {
    name: 'AppMain',
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