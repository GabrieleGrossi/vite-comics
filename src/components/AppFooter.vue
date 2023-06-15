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
<style>
    div.upper-footer{
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;
        color: white;
        font-size: 0.8rem;
        display: flex;
        flex-direction: row;
    }
    div.upper-footer div.link{
        display: flex;
        flex-direction: row;
        width: 60%;
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
    div.upper-footer ul li a {
        color: #858585;
    }
    div.upper-footer img{
        width: 300px;
        height: 300px;
    }
    div.bottom-footer{
        background-color: #303030;
        height: 130px;
        color: white;
    }
</style>