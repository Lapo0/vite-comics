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
                            "thumb": "/public/images/batman.png",
                            "price": "$19.99",
                            "series": "Action Comics",
                            "type": "comic book"
                        },
                        {
                            "thumb": "/public/images/batman.png",
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
            padding-top: 400px;
        }
        .content {
            padding: 40px 0;
            font-size: 40px;
            color: white;
            background-color: $dark-gray;

            .grid {
                display: grid;
                grid-template-columns: repeat(6, 1fr);
                grid-gap: 20px;

            }
        }
    }
    

</style>