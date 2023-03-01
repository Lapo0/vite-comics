<script>
    export default {

    }
</script>

<template>
    <main>
        <div class="container">
        <div class="content">
        <p>
            ciao
        </p>
        </div>
        </div>
    </main>

</template>

<style lang="scss" scoped>

@use '/src/style/partials/_variables.scss' as *;

    main {
        background-color: $dark-gray;
        .content {
            padding: 40px 0;
            font-size: 40px;
            color: white;
        }
    }
    

</style>