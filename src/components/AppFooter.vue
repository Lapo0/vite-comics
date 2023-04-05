<script>
    export default {

    }
</script>

<template>
    <footer>
        <section class="celest">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="item">
                            <div class="item-img">
                                <img src="/public/images/buy-comics-digital-comics.png" alt="">
                            </div>
                            <p>
                                DIGITAL COMICS
                            </p>
                        </div>
                    </div>
                    <div class="col">
                        <div class="item">
                            <div class="item-img">
                                <img src="/public/images/buy-comics-merchandise.png" alt="">
                            </div>
                            <p>
                                DC MERCHANDISE
                            </p>
                        </div>
                    </div>
                    <div class="col">
                        <div class="item">
                            <div class="item-img">
                                <img src="/public/images/buy-comics-subscriptions.png" alt="">
                            </div>
                            <p>
                                SUBSCRIPTION
                            </p>
                        </div>
                    </div>
                    <div class="col">
                        <div class="item">
                            <div class="item-img">
                                <img src="/public/images/buy-comics-shop-locator.png" alt="">
                            </div>
                            <p>
                                COMIC SHOP LOCATOR
                            </p>
                        </div>
                    </div>
                    <div class="col">
                        <div class="item">
                            <div class="item-img svg">
                                <img src="/public/images/buy-dc-power-visa.svg" alt="">
                            </div>
                            <p>
                                DC POWER VISA
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="image-bg">
            <div class="container">
                <div class="big-logo">
                    <img src="/public/images/dc-logo-bg.png" alt="">
                </div>
                <div class="info">
                    <div class="row">
                        <div class="col">
                            <div class="row-column">
                                <div class="col">
                                    <h3>
                                        DC COMICS
                                    </h3>
                                    <ul class="row-column">
                                        <li><a href="">Characters</a></li>
                                        <li><a href="">Comics</a></li>
                                        <li><a href="">Movies</a></li>
                                        <li><a href="">TV</a></li>
                                        <li><a href="">Games</a></li>
                                        <li><a href="">Videos</a></li>
                                        <li><a href="">News</a></li>
                                    </ul>
                                </div>
                                <div class="col">
                                    <h3 class="shop">
                                        SHOP
                                    </h3>
                                    <ul class="row-column">
                                        <li><a href="">Shop DC</a></li>
                                        <li><a href="">Shop DC Collectibles</a></li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="col">
                            <h3>
                                DC
                            </h3>
                            <ul class="row-column">
                                <li><a href="">Terms Of Use</a></li>
                                <li><a href="">Privacy Policy (News)</a></li>
                                <li><a href="">Ad Choices</a></li>
                                <li><a href="">Advertising</a></li>
                                <li><a href="">Jobs</a></li>
                                <li><a href="">Subscriptions</a></li>
                                <li><a href="">Talent Workshop</a></li>
                                <li><a href="">CPSC Cerficates</a></li>
                                <li><a href="">Ratings</a></li>
                                <li><a href="">Shop Help</a></li>
                                <li><a href="">Contact Us</a></li>
                            </ul>
                        </div>
                        <div class="col">
                            <h3>
                                SITES
                            </h3>
                            <ul class="row-column">
                                <li><a href="">DC</a></li>
                                <li><a href="">MAD Magazine</a></li>
                                <li><a href="">DC Kids</a></li>
                                <li><a href="">DC Universe</a></li>
                                <li><a href="">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="gray">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="button">
                            <button>SING-UP NOW!</button>
                        </div>
                    </div>
                    <div class="col">
                        <div class="row social">
                            <div class="col">
                                <h2>
                                    FOLLOW US
                                </h2>
                            </div>
                            <div class="col">
                                <div class="social-icon">
                                    <img src="/public/images/footer-facebook.png" alt="">
                                </div>
                            </div>
                            <div class="col">
                                <div class="social-icon">
                                    <img src="/public/images/footer-twitter.png" alt="">
                                </div>
                            </div>
                            <div class="col">
                                <div class="social-icon">
                                    <img src="/public/images/footer-youtube.png" alt="">
                                </div>
                            </div>
                            <div class="col">
                                <div class="social-icon">
                                    <img src="/public/images/footer-pinterest.png" alt="">
                                </div>
                            </div>
                            <div class="col">
                                <div class="social-icon">
                                    <img src="/public/images/footer-periscope.png" alt="">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
    </footer>

</template>

<style lang="scss">

@use '/src/style/partials/_variables.scss' as *;

    .celest {
        background-color: $celest;
        color: white;

        .container {
            padding: 40px;

            .row {
                gap: 60px;
                justify-content: center;
            }

            .item {
                display: flex;
                align-items: center;

                .item-img {
                    height: 50px;
                    padding-right: 15px;

                    &.svg img{
                        width: 50px;
                    }
                    
                }

                p {
                    font-size: 15px;
                }
            }
        }
    }

    .image-bg {
        background-image: url('/public/images/footer-bg.jpg');
        background-size: cover;
        color: white;
        z-index: -999;
        overflow: hidden;

        .container {
            padding: 40px 0;
            position: relative;

            .big-logo {
                position: absolute;
                top: -90px;
                right: 0;
            }

            .info .row {
                gap: 60px;
                align-items: start;

                h3 {
                    padding: 10px 0;
                    font-size: 20px;

                    &.shop {
                        margin-top: 10px;
                    }

                }

                li {
                    line-height: 25px;
                    color: rgba(255, 255, 255, 0.5);
                    font-size: 14px;

                    &:hover {
                        color: white;
                    }
                }
            }
        }
    }

    .gray {
        background-color: $gray;
        position: relative;
        z-index: 999;
        color: white;

        .container {
            padding: 30px 0;

            .row {
                justify-content: space-between;

                .button button {
                    line-height: 50px;
                    padding: 0 20px;
                    background-color: $gray;
                    border: 2px solid $celest;
                    color: white;
                    font-size: 20px;

                    &:hover {
                        background-color: $celest;
                    }
                }

                .social {
                    h2 {
                        color: $dark-celest;
                        font-weight: bold;
                    }

                    & > * {
                        padding: 15px;
                    }

                    .social-icon:hover {
                        filter: grayscale(100%) brightness(200%);
                    }
                }
            }
        }
    }



</style>