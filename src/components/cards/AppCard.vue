<template>
    <div class="card">
        <div class="singlecard">
            <img :src="thumb" alt="">
        </div>
        <h2>
            {{ series }}
        </h2>
    </div>
</template>
<script>
export default {
    data () {
        return{

        }
    },
    props : {
        thumb: String,
        series: String
    }
}
</script>
<style lang="scss" scoped>
    .card{
        width: calc(100% / 6);
    }
    .card img{
        object-fit: cover;
    }
</style>