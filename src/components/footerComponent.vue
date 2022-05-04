<template>
    <footer>

        <section id="upper-footer">

            <nav>

                <div class="col">

                    <h4>Dc comics</h4>

                    <ul>

                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>

                    </ul>

                    <h4>Shop</h4>

                    <ul>

                        <li>
                            <a href="#">Shop DC</a>
                        </li>
                        <li>
                            <a href="#">Shop DC Collectibles</a>
                        </li>
                        
                    </ul>
                </div>
                
                <div class="col">

                    <h4>Dc</h4>

                    <ul>

                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy Policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>                 

                    </ul>
                    
                </div>

                <div class="col">

                    <h4>Sites</h4>

                    <ul>

                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>

                    </ul>
                
                </div>
            </nav>

            <div>

                <img src="../assets/img/dc-logo-bg.png" alt="Big Dc Logo">

            </div>

        </section>

        <section id="lower-footer">

            <button>Sign up now!</button>

            <nav>

                <h3>Follow us</h3>

                <ul>

                    <li>
                        <a href="#"><img class="social-logo" src="../assets/img/footer-facebook.png" alt="facebook-logo"></a>
                    </li>
                    <li>
                        <a href="#"><img class="social-logo" src="../assets/img/footer-twitter.png" alt="twitter-logo"></a>
                    </li>
                    <li>
                        <a href="#"><img class="social-logo" src="../assets/img/footer-youtube.png" alt="youtube-logo"></a>
                    </li>
                    <li>
                        <a href="#"><img class="social-logo" src="../assets/img/footer-pinterest.png" alt="pinterest-logo"></a>
                    </li>
                    <li>
                        <a href="#"><img class="social-logo" src="../assets/img/footer-periscope.png" alt="periscope-logo"></a>
                    </li>
                </ul>

            </nav>

        </section>

    </footer>
</template>

<script>
    export default {
        name: 'SiteFooter'
    }
</script>

<style lang="scss" scoped>

    @import '@/style/general.scss';


    ul{
        list-style: none;
        li>a{
            text-decoration: none;
            color: $linkColor;
        }
    }
    
    #upper-footer{
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        
        nav{
            display: flex;
            align-content: center;
            flex-basis: 30%;
            padding-left: 20px;
            .col{
                padding: 10px;
                h4{
                    color: $whiteMainColor;
                    padding: 10px 0 ;
                }
                li{  
                    font-size: 0.7rem;
                    padding-bottom: 0.5rem;
                }
            }
            
        }
        
        div{
            height: 350px;
            position: relative;
            flex-basis: 50%;
            img{
                position: absolute;
                width: 90%;
                left: 50%;
                top:50%;
                transform: translate(-50%, -50%);
            }
        }
    }
    #lower-footer{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 25px 155px ;
        background-color: $footerBgColor;
        button{
            padding: 10px;
            background-color: transparent;
            color: $whiteMainColor;
            font-size: 1rem;
            font-weight: 600;
            border: 3.5px solid $mainBlueColor;
        }
        nav{
            display: flex;
            justify-content: center;
            align-items: center;
            h3{
                color: $mainBlueColor;
                padding-right: 20px;
            }
            ul{
                display: flex;
                justify-content: center;
                align-items: center;
                .social-logo{
                    padding: 5px;
                }
            }
        }
    }
</style>