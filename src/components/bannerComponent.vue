<template>

    <section  id="shop-section">
        <ul>
            <li v-for="(item, index) in banner" :key="index">
                <a href="#">
                    <img :src="item.src">
                    <p>{{item.text}}</p>
                </a>
            </li>
                    
        </ul>
    </section>       
    
</template>


<script>

    export default {
        name: 'SiteBanner',
        data(){
            return{
                banner:[
                    {
                        id: 1 ,
                        src: require('@/assets/img/buy-comics-digital-comics.png'),
                        text: 'Digital Comics'
                    },
                    {
                        id: 2 ,
                        src: require('@/assets/img/buy-comics-merchandise.png'),
                        text: 'Dc Merchandise'
                    },
                    {
                        id: 3 ,
                        src: require('@/assets/img/buy-comics-subscriptions.png'),
                        text: 'subscription'
                    },
                    {
                        id: 4 ,
                        src: require('@/assets/img/buy-comics-shop-locator.png'),
                        text: 'comic shop locator'
                    },
                    {
                        id: 5 ,
                        src: require('@/assets/img/buy-dc-power-visa.svg'),
                        text: 'dc power visa'
                    },
                ]
            }
        }
    }

</script>

<style lang="scss" scoped>
@import '@/style/general.scss';
@import '@/style/variables.scss';


#shop-section{
    background-color: $mainBlueColor;
    color : $whiteMainColor;
    height: 150px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    column-gap: 40px;
    ul{
        list-style: none;
        display: flex; 
        gap: 20px;

        a{
            text-decoration: none;
            color : $whiteMainColor;
            text-transform: uppercase;
            display: flex;
            align-items: center;
            margin: 0 15px;
            
            img{
                max-height: 40px;
                &:hover{
                    transition: 1s;
                    max-height: 60px;
               
                 }
            }
            p{
                margin-left: 10px;
                font-size: 0.8rem;
            }
        }
    }
}


</style>
