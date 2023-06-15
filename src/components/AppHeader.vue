<template>
    <header >
        <div id="brand">
            <img src="../assets/img/dc-logo.png" alt="Dc comics logo">
        </div>
        <nav id="top-navbar">
            <ul>
                <li v-for="link in navbarLinks" :class="link.active ? 'active' : ''">
                    <a :href="link.link">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
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
                    active: false
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
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    header{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 70%;
        margin: 0 auto;
        margin-top: 2rem;

        div#brand img{
            height: 70px;
            display: block;
            margin: 0 auto;
        }

        nav#top-navbar ul{
            @include flex();
            flex-direction: row;

            li{
                padding: 1rem;
                font-size: .9rem;
                font-weight: 600;
                transition: background-color 1s ease;
                //margin-bottom: 2rem;
                padding-bottom: 5rem;
                border-bottom: 8px solid white;
                &.active,
                &:hover{
                    border-bottom: 8px solid $accentBg;
                }
            }
        }
    }
</style>    