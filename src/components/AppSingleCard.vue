<template>
    <div>
        <div class='card'>
           <img :src="cardElement.thumb" alt="">
        </div>
        <h3>
            {{cardElement.series}}
        </h3>
    </div>
</template>
<script>

export default {
    name: 'SingleCard',
    props: {
        cardElement : String
    }
}
</script>
<style lang="scss" scoped>
    div.card{
        width: calc(100% / 6);
    }
</style>