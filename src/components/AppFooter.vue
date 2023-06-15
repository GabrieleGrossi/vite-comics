<template>
    <div class="upper-footer">
        <ul>
            <h2>
                DC COMICS
            </h2>
            <li v-for="link in footerLinks">
                <a :href="link.link">
                    {{ link.text }}
                </a>
            </li>
        </ul>
    </div>
    <div class="bottom-footer">
        buttons
    </div>
</template>
<script>
export default {
    name: 'AppFooter',
    data(){
        return{
            footerLinks : [
                {
                    link: '#',
                    text: 'Characters',
                },
                {
                    link: '#',
                    text: 'Comics',
                },
                {
                    link: '#',
                    text: 'Movies',
                },
                {
                    link: '#',
                    text: 'Tv',
                },
                {
                    link: '#',
                    text: 'Games',
                },
                {
                    link: '#',
                    text: 'Collectibles',
                },
                {
                    link: '#',
                    text: 'Videos',
                },
                {
                    link: '#',
                    text: 'News',
                    active: false
                }
            ]
        }
    }
}
</script>
<style>
    div.upper-footer{
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;
        color: white;
        font-size: 0.8rem;
    }
    div.upper-footer ul li a {
        color: #858585;
    }
    div.bottom-footer{
        background-color: #303030;
        height: 130px;
        color: white;
    }
</style>