<script>
    export default {

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
                    <li>
                        <a href="#">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="#">COMISCS</a>
                    </li>
                    <li>
                        <a href="#">MOVIES</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">GAMES</a>
                    </li>
                    <li>
                        <a href="#">COLLECTIBLES</a>
                    </li>
                    <li>
                        <a href="#">VIDEOS</a>
                    </li>
                    <li>
                        <a href="#">FANS</a>
                    </li>
                    <li>
                        <a href="#">NEWS</a>
                    </li>
                    <li>
                        <a href="#">SHOP</a>
                    </li>
                </ul>
            </div>
        </div>
        

    </div>
</template>

<style lang="scss" scoped>

@use 'src/style/partials/_variables.scss' as *;

    .row {
        justify-content: space-between;

        .link {
            display: flex;

            li {
                line-height: 40px;
                margin: 0 20px;
                font-weight: bold;
                position: relative;

                &::before {
                content: '';
                position: absolute;
                bottom: 0;
                left: 0;
                width: 100%;
                height: 2px;
                background-color: $celest;
                opacity: 0;
                }
                
                &:hover {
                    color: $celest;
                }
                &:hover::before {
                opacity: 1;
                }

                
            }
        }
    }

    


</style>

