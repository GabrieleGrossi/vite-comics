<template>
    <div class="card">
        <div class="singlecard">
            <img :src="thumb" alt="">
        </div>
        <h4>
            {{ series }}
        </h4>
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
        width: calc((100% / 6) - 1.5rem);
        margin-left: 1.5rem;
        margin-bottom: 1.5rem;
        margin-top: 2rem;
    }
    .card img{
        object-fit: cover;
        height: 250px;
    }
    h4{
        text-transform: uppercase;
    }
</style>