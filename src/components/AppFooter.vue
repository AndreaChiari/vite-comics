<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <div class="container-index">
            <section class="index-recap">
                <div class="row">
                    <div class="column">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h2>SHOP</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                        </ul>
                    </div>
                    <div class="column">
                        <h2>DC</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                    <div class="column">
                        <h2>SITES</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                </div>
                <figure>
                    <img class="img-jumbotron" src="../assets/img/dc-logo.png" alt="dc-logo.png">
                </figure>
            </section>
        </div>
        <div class="navbar-footer">
            <section>
                <button type="button">SIGN UP NOW!</button>
                <div>
                    <h2>FOLLOW US</h2>
                    <figure class="">
                        <a href="">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </a>
                    </figure>
                    <figure class="">
                        <a href="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </a>
                    </figure>
                    <figure class="">
                        <a href="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </a>
                    </figure>
                    <figure class="">
                        <a href="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </a>
                    </figure>
                    <figure class="">
                        <a href="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </a>
                    </figure>
                </div>
            </section>
        </div>
    </footer>
</template>





<style scoped lang="scss">
@use '../assets/scss/colors.scss' as *;
@use '../assets/scss/mixin.scss' as *;

.container-index {
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .index-recap {
        @include container;
        display: flex;

        a {
            color: $color-white;
            text-decoration: none;
        }

        .row {
            width: calc(100% / 2);
            display: flex;
            gap: 30px;
            padding-top: 30px;

            .column {
                h2 {
                    color: $color-white ;
                    margin-bottom: 10px;
                }

                ul {
                    list-style-type: none;
                    margin-bottom: 30px;
                }
            }
        }

    }

}

figure {
    display: flex;
    align-items: center;
    justify-content: center;
    padding-left: 10px;
    width: 500px;

    .img-jumbotron {
        width: 400px;
        transform: rotate(-30deg);
        opacity: 0.6;
        object-position: 10%;
    }

}

.navbar-footer {
    height: 150px;
    background-color: rgb(48, 48, 48);

    section {
        @include container;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        div {
            display: flex;
            justify-content: center;
            align-items: center;

            figure {
                height: 80px;
                width: 50px;
            }
        }

        button {
            border: 1px solid $color-blue;
            padding: 10px;
            background-color: rgb(48, 48, 48);
            color: $color-white;
            cursor: pointer;
        }

        h2 {
            color: $color-blue ;
        }
    }

}
</style>
    

