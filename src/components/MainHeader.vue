<template>
    <header>
        <div class="container">
            <div class="logo" >
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav class="nav">
               <ul>
                    <li v-for="(el, index) in links" 
                    :key="index"
                    :class="{'active' : el.active}">
                        <a :href="el.url">{{el.text}}</a>
                    </li>
                    
               </ul>
    
            </nav>            
        </div>
    </header>
</template>


<script>
export default {
  name: 'MainHeader',
  data() {
        return{
            links:[
                {
                text:"CHARACTERS",
                url:"#",
                active: false
                },
                {
                text:"COMICS",
                url:"#",
                active: true
                },
                {
                text:"MOVIES",
                url:"#",
                active: false
                },
                {
                text:"TV",
                url:"#",
                active: false
                },
                {
                text:"GAMES",
                url:"#",
                active: false
                },
                {
                text:"COLLECTIBLES",
                url:"#",
                active: false
                },
                {
                text:"VIDEOS",
                url:"#",
                active: false
                },
                {
                text:"FANS",
                url:"#",
                active: false
                },
                {
                text:"NEWS",
                url:"#",
                active: false
                },
                {
                text:"SHOP",
                url:"#",
                active: false
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    
    @import '../style/variables.scss';

    header{
        background: white;
    }
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
   
        .logo{
            text-align: center;
            padding: 1.2rem 0;
        }
        .nav ul{
            display: flex;
            align-items: center;
            justify-content: center;

            li{
                font-weight: 600;
                padding: 3.7rem 0.9rem;
                border-bottom: 5px solid transparent;
                
                &.active, &:hover{
                    border-bottom-color: $main-color;
                }
            }
        }
    }
</style>