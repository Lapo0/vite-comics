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
        font-size: 16px;
        text-transform: uppercase;
        padding-top: 10px;
    }

        img {
            max-width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            object-position: center;

            &:hover {
            filter: drop-shadow(16px 16px 20px black);
            transform: scale(1.1);
            }
        }


   


</style>