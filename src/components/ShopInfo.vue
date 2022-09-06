<template>
    <section class="shop-section">
        <div class="container">
            <div class="info-shop">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <div class="shop-text"> DIGITAL COMICS </div>
            </div>
            <div class="info-shop">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <div class="shop-text"> DC MERCHANDISE </div>
            </div>
            <div class="info-shop">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <div class="shop-text"> SUBSCRIPTION </div>
            </div>
            <div class="info-shop">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <div class="shop-text"> COMIC SHOP LOCATOR </div>
            </div>
            <div class="info-shop visa">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <div class="shop-text"> DC POWER VISA </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ShopInfo',
    props:{
        src: String,
        url: String,
        text: String,
        svg: Boolean
    },
    data() {
        return{
            blueShop:[
                {
                    icon:'../assets/img/buy-comics-digital-comics.png',
                    url:'#',
                    text:'digital comics',
                    svg: false
                },
                {
                    icon:'../assets/img/buy-comics-merchandise.png',
                    url:'#',
                    text:'dc merchandise',
                    svg: false
                },
                {
                    icon:'../assets/img/buy-comics-subscriptions.png',
                    url:'#',
                    text:'subscription',
                    svg: false
                },
                {
                    icon:'../assets/img/buy-comics-shop-locator.png',
                    url:'#',
                    text:'comic shop locator',
                    svg: false
                },
                {
                    icon:'../assets/img/buy-dc-power-visa.svg',
                    url:'#',
                    text:'dc power visa',
                    svg: true
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    @import '../style/shop-info.scss';


</style>