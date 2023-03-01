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
                <p>
                    ciao
                </p>
            </div>
        </section>
        <section class="gray">
            <div class="container">
                <p>
                    ciao
                </p>
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
        .container {
            padding: 40px 0;
        }
    }

    .gray {
        background-color: $gray;
        .container {
            padding: 40px 0;
        }
    }



</style>