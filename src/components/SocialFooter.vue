<template>
    <section>

        <div class="container">
            <div class="sign-up">  
                <input class="btn" type="submit" value="SIGN-UP NOW!">
            </div>
            <div class="social-nav">
                <div class="follow"> FOLLOW US</div>
                <div class="social-icon">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </div>
                <div class="social-icon">
                    <img src="../assets/img/footer-twitter.png" alt="">
                </div>
                <div class="social-icon">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </div>
                <div class="social-icon">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                </div>
                <div class="social-icon">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>

    </section>
</template>

<script>

export default {
    name: 'SocialFooter',
}
</script>

<style lang="scss" scoped>

    @import '../style/variables.scss';

    section{
        background-color: $footer-bg;
        
        .container{
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px 1.5rem;
            z-index: 999;
    
            .btn{
                background-color: transparent;
                border: solid $main-color;
                padding: 10px;
                color: white;
                font-weight: 600;
                cursor: pointer;
                transition: linear 0.2s;
    
                &:hover{
                    background-color: $main-color;
                }
            }
    
            .social-nav{
                display: flex;
                align-items: center;
                gap: 1.5rem;
                z-index: 999;
    
                .follow{
                    color: $main-color;
                    font-weight: 600;
                    font-size: 1.2rem;
                }
                .social-icon{
                    cursor: pointer;

                    &:hover img{
                        transition: all 0.2s ease-in-out;
                        transform: scale(1.1);

                    }
                }
            }
    
        }
    }


</style>