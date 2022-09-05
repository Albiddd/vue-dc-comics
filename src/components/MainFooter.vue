<template>
    <footer>

        <div class="container">
            <div class="footer-nav">
                <ul>
                    <li> <h3>DC COMICS</h3> </li>
                    <li v-for="(el, index) in ComicsLinks" 
                    :key="index">
                        <a :href="el.url">{{el.text}}</a>
                    </li>

                    <li> <h3>SHOP</h3> </li>
                    <li v-for="(el, index) in ShopLinks" 
                    :key="index">
                        <a :href="el.url">{{el.text}}</a>
                    </li>
                    
                </ul>

                <ul>
                    <li> <h3>DC</h3> </li>
                    <li v-for="(el, index) in DcLinks" 
                    :key="index">
                        <a :href="el.url">{{el.text}}</a>
                    </li>
                </ul>

                <ul>
                    <li> <h3>Sites</h3> </li>
                    <li v-for="(el, index) in SitesLinks" 
                    :key="index">
                        <a :href="el.url">{{el.text}}</a>
                    </li>
                </ul>

            </div>
            <div class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>

    </footer>
</template>

<script>
export default {
    name: 'MainFooter',
    data() {
        return{
            ComicsLinks:[
                {
                text:"Characters",
                url:"#",
                },
                {
                text:"Comics",
                url:"#",
                },
                {
                text:"Movies",
                url:"#",
                },
                {
                text:"TV",
                url:"#",
                },
                {
                text:"Games",
                url:"#",
                },
                {
                text:"Collectibles",
                url:"#",
                },
                {
                text:"Videos",
                url:"#",
                },
                {
                text:"News",
                url:"#",
                }
            ],
            DcLinks:[
                {
                text:"Terms Of Use",
                url:"#",
                },
                {
                text:"Privacy policy(New)",
                url:"#",
                },
                {
                text:"Ad Choices",
                url:"#",
                },
                {
                text:"Advertisig",
                url:"#",
                },
                {
                text:"Jobs",
                url:"#",
                },
                {
                text:"Subscription",
                url:"#",
                },
                {
                text:"Talent Workshops",
                url:"#",
                },
                {
                text:"CPSC Certificates",
                url:"#",
                },
                {
                text:"Ratings",
                url:"#",
                },
                {
                text:"Shop Help",
                url:"#",
                },
                {
                text:"Contact Us",
                url:"#",
                }
            ],
            SitesLinks:[
                {
                text:"DC",
                url:"#",
                },
                {
                text:"MAD Magazine",
                url:"#",
                },
                {
                text:"DC Kids",
                url:"#",
                },
                {
                text:"DC Universe",
                url:"#",
                },
                {
                text:"DC Power Visa",
                url:"#",
                },            
            ],
            ShopLinks:[
                {
                text:"DC",
                url:"#",
                },
                {
                text:"MAD Magazine",
                url:"#",
                },       
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    @import '../style/main-footer.scss';


</style>