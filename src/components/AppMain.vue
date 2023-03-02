<script>
    import Card from '/src/components/Card.vue'

    export default {
        components: {
            Card
        },
        data() {
            return {
                card: [
                        {
                            "thumb": "data:image/jpeg;base64,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",
                            "price": "$19.99",
                            "series": "Action Comics",
                            "type": "comic book"
                        },
                        {
                            "thumb": "data:image/jpeg;base64,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",
                            "series": "American Vampire 1976",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Aquaman",
                            "type": "graphic novel"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batgirl",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman Beyond",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman/Superman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman/Superman Annual",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman: The Joker War Zone",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman: Three Jokers",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Batman: White Knight Presents: Harley Quinn",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
                            "series": "Catwoman",
                            "type": "graphic novel"
                        }
                    ]
            }
        },

    }
</script>

<template>
    <main>
        <div class="jumbotron">
            <div class="content">
                <div class="container">
                    <ul class="grid">
                        <Card v-for="el in card" :key="el.thumb" :thumb="el.thumb" :series="el.series" />
                    </ul>
                    <div class="series-button">
                        <button>
                            CURRENT SERIES
                        </button>
                    </div>
                    <div class="load-button">
                        <button>
                            LOAD MORE
                        </button>
                    </div>
                </div>
            </div>
        </div>
        
    </main>

</template>

<style lang="scss" scoped>

@use '/src/style/partials/_variables.scss' as *;

    main {
        background-color: $dark-gray;

        .jumbotron {
            background-image: url(/public/images/jumbotron.jpg);
            background-position: center;
            background-size: cover;
            padding-top: 400px;

            .content {
                font-size: 40px;
                color: white;
                background-color: $dark-gray;

                .container {
                    position: relative;

                    .grid {
                        padding: 60px 0;
                        display: grid;
                        grid-template-columns: repeat(6, 1fr);
                        gap: 50px 20px;
                    }

                    .series-button {
                        position: absolute;
                        top: -25px;

                        button {
                            font-size: 25px;
                        }
                    }

                    .load-button {
                        text-align: center;
                        padding-bottom: 20px;

                        button {
                            font-size: 15px;
                            width: 200px;
                        }
                    }

                    button {
                        background-color: $celest;
                        border: 0;
                        line-height: 50px;
                        padding: 0 25px;
                        color: white;

                        &:hover {
                            transform: scale(1.1);
                        }
                    }
                }
            }
        }
        
    }
    

</style>