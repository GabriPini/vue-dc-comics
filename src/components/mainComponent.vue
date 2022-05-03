<template>
    <main>
        <section id="jumbotron">
            <h3> -- Content goes here -- </h3>
        </section>

        <section  id="shop-section">
                <ul>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <p>digital comics</p>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <p>dc merchandise</p>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <p>subscription</p>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <p>comic shop locator</p>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <p>dc power visa</p>
                        </a>
                    </li>
                </ul>
        </section>       
            
    </main>
</template>

<script>


export default {
    name: 'SiteMain',
}
</script>

<style lang="scss" scoped>
@import '@/style/general.scss';
@import '@/style/variables.scss';

#jumbotron{
   background-color: $contentBgColor;
    height: 100px;

    h3{
        color: $whiteMainColor;
        padding: 2.5rem 13rem;
    }
}

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
        gap: 50px;

        a{
            text-decoration: none;
            color : $whiteMainColor;
            text-transform: uppercase;
            display: flex;
            align-items: center;
            margin: 0 15px;
            
            img{
                max-height: 40px;
            }
            p{
                margin-left: 10px;
                font-size: 0.8rem;
            }
        }
    }
}


</style>