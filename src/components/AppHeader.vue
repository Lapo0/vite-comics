<script>
    export default {
        data() {
            return {
                menu: [  'CHARACTERS',  'COMICS',  'MOVIES',  'TV',  'GAMES',  'COLLECTIBLES',  'VIDEOS',  'FANS',  'NEWS',  'SHOP'],
                activeIndex: '',
            }
        },
        methods: {
            linkActive(index) {
                
            }
        },

    }

</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col">
                <div class="logo">
                    <img src="/public/images/dc-logo.png" alt="">
                </div>
            </div>
            <div class="col">
                <ul class="link">
                    <li
                    v-for="(link, index) in menu"
                    >
                        <a href="#">{{ link }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

@use 'src/style/partials/_variables.scss' as *;

    .container {
        .row {
        justify-content: space-between;
        align-items: stretch;

            .logo {
                padding: 20px 0;
            }

            .link {
                display: flex;
                height: 100%;

                li {
                    line-height: 40px;
                    margin: 0 15px;
                    font-weight: bold;
                    font-size: 13px;
                    position: relative;
                    height: 100%;
                    display: flex;
                    align-items: center;

                    &::before {
                    content: '';
                    position: absolute;
                    bottom: 0;
                    left: 0;
                    width: 100%;
                    height: 5px;
                    background-color: $celest;
                    opacity: 0;
                    }
                    
                    &:hover, &.active {
                        color: $celest;
                    }
                    &:hover::before, &.active::before {
                    opacity: 1;
                    }
                }
            }
        }
    }

    
</style>

