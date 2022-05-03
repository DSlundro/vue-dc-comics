<template>
    <footer>
        <div class="f-bg">
            <div class="container">
                <div class="row py-5">

                    <div class="col-2">
                        
                        <div>
                            <h4 class="text-white">DC COMICS</h4>
                            <ul class="p-0">
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                        </div>

                        <div>
                            <h4 class="text-white">SHOP</h4>
                            <ul class="p-0">
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-2">
                        <div>
                            <h4 class="text-white">DC</h4>
                            <ul class="p-0">
                                <li>Terms Of Use</li>
                                <li>Privacy policy (New)</li>
                                <li>Ad Choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscriptions</li>
                                <li>Talent Workshop</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop Help</li>
                                <li>Contact Us</li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-2">
                        <div>
                            <h4 class="text-white">SITES</h4>
                            <ul class="p-0">
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Universe</li>
                                <li>DC Power Visa</li>
                            </ul>
                        </div>
                    </div>

                    <div class="dc-bg col-6 d-flex justify-content-end">
                        <img src="@/assets/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </div>

        <div class="contact">
            <div class="container">
                <div class="row">
                    <div class="col-3 d-flex align-items-center">
                        <button type="button" class="btn">SIGN-UP NOW!</button>
                    </div>

                    <div class="col-9 d-flex justify-content-end align-items-center">
                        <div class="follow-us px-2 pt-1">
                            <a href="#">FOLLOW US</a>
                        </div>

                        <div class="social d-flex ps-2 align-items-center">
                            <a href="#"><img src="@/assets/img/footer-facebook.png" alt=""></a>
                            <a href="#"><img src="@/assets/img/footer-twitter.png" alt=""></a>
                            <a href="#"><img src="@/assets/img/footer-youtube.png" alt=""></a>
                            <a href="#"><img src="@/assets/img/footer-pinterest.png" alt=""></a>
                            <a href="#"><img src="@/assets/img/footer-periscope.png" alt=""></a>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
    
}
</script>

<style lang="scss" scoped>
footer{
    .f-bg{
        background-image: url(@/assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: 100%;
        }
    button{
        color: white;
        font-weight: bold;
        border: 3px solid #0282F9;
    }
    li{
        list-style: none; 
        color: gray;
        &hover{color: white;}
        }
    h4{font-weight: bold;}
    .dc-bg{
        img{
        width: 600px;
        position: absolute;
        transform: translate(0, -150px);
        }
    }
    .contact{
        position: relative;
        z-index: 1;
        background-color: #303030;
        width: 100%;

        .follow-us a{
            color: #0282F9;
        }

        .col-9{height: 100px;
            .social{
                position: relative;
                img{width: 22px;}
                a{padding: 0 5px;}
            }
        }
    }
}
</style>