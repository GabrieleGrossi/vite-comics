<template>
    <div class="upper-footer">
        <div class="link">
            <div>
                <ul>
                    <h2>
                        DC COMICS
                    </h2>
                    <li v-for="link in footerLinks">
                        <a :href="link.link">
                            {{ link.text }}
                        </a>
                    </li>
                    <h2>
                        SHOP
                    </h2>
                    <li v-for="link in shopLinks">
                        <a :href="link.link">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
            <div>
                <ul>
                    <h2>
                        DC
                    </h2>
                    <li v-for="link in dcLinks">
                        <a :href="link.link">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
            <div>
                <ul>
                    <h2>
                        SITES
                    </h2>
                    <li v-for="link in sitesLinks">
                        <a :href="link.link">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <img src="../assets/img/dc-logo-bg.png" alt="Dc comics logo">
    </div>
    <div class="bottom-footer">        
        <div class="container">
            <div>
                <button>
                    SIGN-UP NOW!
                </button>
            </div>
            <div class="flex">
                <h2>
                    FOLLOW US
                </h2>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
            </div>
        </div>
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
                }
            ],
            shopLinks : [
                {
                    link: '#',
                    text: ' Shop DC'
                },
                {
                    link: '#',
                    text: ' Shop DC Collectibles'
                }
            ],
            dcLinks : [
                {
                    link: '#',
                    text: 'Terms Of Use',
                },
                {
                    link: '#',
                    text: 'Privacy policy (New)',
                },
                {
                    link: '#',
                    text: 'Ad Choices',
                },
                {
                    link: '#',
                    text: 'Advertising',
                },
                {
                    link: '#',
                    text: 'Jobs',
                },
                {
                    link: '#',
                    text: 'Subscritions',
                },
                {
                    link: '#',
                    text: 'Talent Workshop',
                },
                {
                    link: '#',
                    text: 'CPSC Certicates',
                },
                {
                    link: '#',
                    text: 'Ratings',
                },
                {
                    link: '#',
                    text: 'Shop Help',
                },
                {
                    link: '#',
                    text: 'Contact Us',
                }
            ],
            sitesLinks : [
                {
                    link: '#',
                    text: 'DC',
                },
                {
                    link: '#',
                    text: 'MAD Magazine',
                },
                {
                    link: '#',
                    text: 'DC Kids',
                },
                {
                    link: '#',
                    text: 'DC Universe',
                },
                {
                    link: '#',
                    text: 'DC Power Visa',
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;   
    div.upper-footer{
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        height: 400px;
        color: white;
        font-size: 0.8rem;
        display: flex;
        flex-direction: row;
    }
    div.upper-footer div.link{
        display: flex;
        flex-direction: row;
        width: 30%;
        margin: 0 auto;
    }

    div.upper-footer div.link div{
        margin: 0 auto;
    }
    div.upper-footer div ul h2{
        margin-top: 0.5rem;
    }
    div.upper-footer div ul li{
        margin-top: 0.3rem;
    }
    div.upper-footer div ul li :hover{
        color: white;
    }    
    div.upper-footer ul li a {
        color: #858585;
    }
    div.upper-footer img{
        width: 400px;
        height: 400px;
        margin: 0 auto;
    }
    div.bottom-footer{
        background-color: #303030;
        height: 130px;
        color: white;
    }
    div.bottom-footer div.container{
        width: 70%;
        display: flex;
        justify-content: space-between;
        margin: 0 auto;
    }
    div.bottom-footer div.container button{
        background-color: transparent;
        border: 2px solid $accentBg;
        color: white;
        padding: 0.8rem;
    }
    div.bottom-footer div.container{
        color: $accentBg;
        padding-top: 3rem;
    }
    div.flex img{
        width: 40px;
        height: 40px;
        align-items: center;
        justify-content: center;
        margin-left: 0.5rem;
    }
</style>