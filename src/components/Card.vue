<script>
    export default {
        props: {
            thumb: String,
            series: String,
        }

    }
</script>

<template>

    <li>
        <img :src="thumb" alt="">
        <div class="text">
            <h4>
                {{ series }}
            </h4>
        </div>

    </li>

</template>

<style lang="scss" scoped>

</style>