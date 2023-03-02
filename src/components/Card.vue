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
        <div class="img">
            <img :src="thumb" alt="">
        </div>
        <div class="text">
            <p>
                {{ series }}
            </p>
        </div>

    </li>

</template>

<style lang="scss" scoped>

    p {
        font-size: 18px;
    }

        img {
            max-width: 100%;
        }

        img:hover {
            filter: drop-shadow(16px 16px 20px black);
            transform: scale(1.1);
        }

   


</style>