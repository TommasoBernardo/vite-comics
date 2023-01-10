<script>
    export default {
        name: 'AppFooter'
    }
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer-list">

                <div>
                    <h3 class="color">DC COMICS</h3>
                        <ul> 
                                <li ><a class="color-grey" href="">Characters</a></li>
                                <li><a class="color-grey" href="">Comics</a></li>
                                <li><a class="color-grey" href="">Movies</a></li>
                                <li><a class="color-grey" href="">TV</a></li>
                                <li><a class="color-grey" href="">Games</a></li>
                                <li><a class="color-grey" href="">Videos</a></li>
                                <li><a class="color-grey" href="">News</a></li>
                            </ul>

                <h3>SHOP</h3>
                <ul> 
                    <li><a class="color-grey" href="">Shop DC</a></li>
                    <li><a class="color-grey" href="">Shop DC Collectibles</a></li>
                </ul>
               </div>

               <div>
                <h3>DC</h3>
                <ul> 
                    <li><a class="color-grey" href="">Terms Of Use</a></li>
                    <li><a class="color-grey" href="">Privacy policy(New)</a></li>
                    <li><a class="color-grey" href="">Ad Choise</a></li>
                    <li><a class="color-grey" href="">Adverting</a></li>
                    <li><a class="color-grey" href="">Jobes</a></li>
                    <li><a class="color-grey" href="">Subscriptions</a></li>
                    <li><a class="color-grey" href="">Talent Workshop</a></li>
                    <li><a class="color-grey" href="">CPSC Certificaces</a></li>
                    <li><a class="color-grey" href="">Ratings</a></li>
                    <li><a class="color-grey" href="">Shop Help</a></li>
                    <li><a class="color-grey" href="">Contacts Us</a></li>
                </ul>
               </div>

               <div>
                <h3>SITES</h3>
                <ul> 
                    <li><a class="color-grey" href="">DC</a></li>
                    <li><a class="color-grey" href="">MAQ Magazine</a></li>
                    <li><a class="color-grey" href="">DC Kids</a></li>
                    <li><a class="color-grey" href="">DC Universe</a></li>
                    <li><a class="color-grey" href="">DC Power Visa</a></li>
                </ul>
               </div>

            </div>
            <div class="dc-logo-bg">
            </div>
        </div>

        <section id="footer-contact">
            <div class="container">
                <div class="button">
                    SIGN-UP NOW
                </div>

                <div>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </div>
            </div>
        </section>
    </footer>
</template>



<style lang="scss" scoped>
footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white;
    
    .container{
        margin: 0 auto;
        width: 80%;
        display: flex;
        justify-content: space-between;
    }
    .footer-list{
        padding: 30px 0;
        display: flex;
        gap: 10px;
        ul{
            font-size: 14px;
        }
    .dc-logo-bg{
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        width: 50%;
    }
    #footer-contact{
        background-color: black;
        padding: 35px 0;
        .button{
            padding: 15px;
            border: 1px solid rgb(49, 126, 235);
        }
        .footer-social{
            display: flex;
            gap: 10px;
            align-items: center;
        }
    }
}
}
</style>