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
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",
                            "price": "$19.99",
                            "series": "Action Comics",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$3.99",
                            "series": "American Vampire 1976",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$16.99",
                            "series": "Aquaman",
                            "type": "graphic novel"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$2.99",
                            "series": "Batgirl",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$3.99",
                            "series": "Batman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$2.99",
                            "series": "Batman Beyond",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$3.99",
                            "series": "Batman/Superman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$4.99",
                            "series": "Batman/Superman Annual",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$5.99",
                            "series": "Batman: The Joker War Zone",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$6.99",
                            "series": "Batman: Three Jokers",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$4.99",
                            "series": "Batman: White Knight Presents: Harley Quinn",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQY77OMiWjJS3OUxL-_9E1GJiCDLZzdQmoobg&usqp=CAU",                            "price": "$16.99",
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