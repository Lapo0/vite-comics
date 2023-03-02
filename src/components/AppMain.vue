<script>
    import Card from '/src/components/Card.vue'

    export default {

    }
</script>

<template>
    <main>
        <div class="jumbotron">
            <div class="content">
                <div class="container">


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
        }
    }
    

</style>