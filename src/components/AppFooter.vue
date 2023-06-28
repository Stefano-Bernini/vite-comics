<script>
export default {
    
    data(){
        return{
            blueInfos : [
                {
                    immg: './src/assets/img/buy-comics-digital-comics.png',
                    lable: 'digital comics'
                },
                {
                    immg: './src/assets/img/buy-comics-merchandise.png',
                    lable: 'dc merchandise'
                },
                {
                    immg: './src/assets/img/buy-comics-subscriptions.png',
                    lable: 'subscription'
                },
                {
                    immg: './src/assets/img/buy-comics-shop-locator.png',
                    lable: 'comic shop locator'
                },
                {
                    immg: './src/assets/img/buy-dc-power-visa.svg',
                    lable: 'dc power visa'
                }
            ],

            objs : [
                {
                    label: 'Character',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Comics',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Movies',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Tv',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Games',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Collectibles',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Videos',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Fans',
                    link: '#',
                    acive: false
                },
                {
                    label: 'News',
                    link: '#',
                    acive: false
                },
            ],

            list:[
                {
                    label: 'Shop DC',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Shop DC Collectibles',
                    link: '#',
                    acive: false
                },
            ],

            dc:[
                {
                    label: 'Term of Use',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Pravacy policy (New)',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Ad Choices',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Advertising',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Jobs',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Subscriptions',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Talent Workshops',
                    link: '#',
                    acive: false
                },
                {
                    label: 'CPSC Certificates',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Ratings',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Shop Help',
                    link: '#',
                    acive: false
                },
                {
                    label: 'Contact us',
                    link: '#',
                    acive: false
                },   
            ],

            sites:[
                {
                    label: 'DC',
                    link: '#',
                    acive: false
                },
                {
                    label: 'MAD Magazine',
                    link: '#',
                    acive: false
                },
                {
                    label: 'DC Kids',
                    link: '#',
                    acive: false
                },
                {
                    label: 'DC Universe',
                    link: '#',
                    acive: false
                },
                {
                    label: 'DC Power Visa',
                    link: '#',
                    acive: false
                },
            ],

            imgs:[
                {
                    src : '../src/assets/img/footer-facebook.png',
                    link: '#',
                    lable: 'Facebook'
                },
                {
                    src : '../src/assets/img/footer-twitter.png',
                    link: '#',
                    lable: 'Twitter'
                },
                {
                    src : '../src/assets/img/footer-youtube.png',
                    link: '#',
                    lable: 'Youtube'
                },
                {
                    src : '../src/assets/img/footer-pinterest.png',
                    link: '#',
                    lable: 'Pinterest'
                },
                {
                    src : '../src/assets/img/footer-periscope.png',
                    link: '#',
                    lable: 'Periscope'
                },
            ]
        }
    }
    
}
</script>

<template>
    <footer>
        <div class="jumbotron-blue">
            <div class="container container-blue">
                <div class="content">
                    <ul class="flex">
                        <li :key="index" v-for="(blueInfos, index) in blueInfos" class="flex align-center">
                            <div class="img-container pointer">
                                <img :src="blueInfos.immg" :alt="blueInfos.lable">
                            </div>
                            <h4 class="uppercase pointer white">{{ blueInfos.lable }}</h4>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="jumbotron">
            <div class="container">
                <div class="dc-background">
                    <div class="col flex p-top-footer">
                        <div class="footer-one">
                            <h2 class="uppercase">dc comics</h2>
                            <ul>
                                <li v-for="(obj, index) in objs" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                            <h2 class="mt uppercase">shop</h2>
                            <ul>
                                <li v-for="(obj, index) in list" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="footer-two">
                            <h2 class="uppercase">dc</h2>
                            <ul>
                                <li v-for="(obj, index) in dc" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="footer-three">
                            <h2 class="uppercase">site</h2>
                            <ul>
                                <li v-for="(obj, index) in sites" :key="index">
                                    <a :href="obj.link" >{{ obj.label }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    
                </div>
            </div>
        </div>
        <div class="jumbotron-social">
            <div class="container">
                <div class="flex between-align">
                    <div class="">
                        <button class="uppercase btn">sign-up now!</button>
                    </div>
                    <div class="flex align-center">
                        <h2 class="uppercase follow">follow us</h2>
                        <ul class="flex">
                            <li class="social-footer-list" v-for="(img, index) in imgs" :key="index">
                                <div>
                                    <a :href="img.link" :key="index"><img :src="img.src" :alt="img.lable"></a>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    .jumbotron-blue {
        background-color: rgb(27, 114, 232);
        padding: 50px 0px;
    }

    .container-blue {
        max-width: 1170px;
    }

    .img-container {
        width: 20%;
    }

    .jumbotron{
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .jumbotron-social{
        background-color: rgb(48,48,48);
        padding: 30px 0px;
    }
    h2{
        margin-bottom: 10px;
        color: white;
    }
    li{
        margin-bottom: 5px;
    }
    a{
        color: grey;
    }
    a:hover{
        color: white;
    }
    .mt{
        margin-top: 30px;
    }
    .footer-three, .footer-two{
        margin-left: 50px;
    }
    .mt{
        margin-top: 50px;
    }
    .dc-background{
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right top 50%;
        padding-bottom: 70px;
    }
    .p-top-footer{
        padding-top: 50px;
    }
    .btn{
        border: 1px solid rgb(27, 114, 232);
        padding: 8px 15px;
        background-color: transparent;
        color: white;
        font-weight: 600;
    }
    .follow{
        color: rgb(27, 114, 232);
        font-weight: 600;
        margin-right: 30px;
    }
    .social-footer-list{
        margin-left: 15px;
    }
</style>