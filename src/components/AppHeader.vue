<template>
    <div class="flex">
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="link in navbarLinks" :class="link.active ? 'active' : ''">
                    <a :href="link.link">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>
<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            navbarLinks : [
                {
                    link: '#',
                    text: 'Characters',
                    active: false
                },
                {
                    link: '#',
                    text: 'Comics',
                    active: true
                },
                {
                    link: '#',
                    text: 'Movies',
                    active: false
                },
                {
                    link: '#',
                    text: 'Tv',
                    active: false
                },
                {
                    link: '#',
                    text: 'Games',
                    active: false
                },
                {
                    link: '#',
                    text: 'Collectibles',
                    active: true
                },
                {
                    link: '#',
                    text: 'Videos',
                    active: false
                },
                {
                    link: '#',
                    text: 'Fans',
                    active: false
                },
                {
                    link: '#',
                    text: 'News',
                    active: false
                },
                {
                    link: '#',
                    text: 'Shop',
                    active: false
                },
            ]

        }
    }
}
</script>
<style lang="scss" scoped>
    .flex{
        display: flex;
    }
    li{
        list-style-type: none;
        display: flex;
        flex-direction: row;
    }
</style>    