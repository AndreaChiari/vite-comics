<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            HeaderList: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],

        }

    }
}
</script>

<template>
    <header>
        <div>
            <figure>
                <img src="../assets/img/dc-logo.png" alt="dc-logo.png">
            </figure>
            <ul>
                <li v-for="list in HeaderList" :key="HeaderList.text"><a href="#">{{ list.text }}</a></li>
            </ul>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../assets/scss/colors.scss' as *;
@use '../assets/scss/mixin.scss' as *;

div {
    @include container;
    margin-top: 10px;
    display: flex;
    align-items: center;
    height: 100px;

    figure {
        width: 20%;

        img {
            @include img-fluid;
        }
    }

    ul {
        display: flex;
        margin-left: 500px;
        list-style-type: none;

        li {
            margin-left: 10px;

            a {
                color: $color-black;
                text-decoration: none;

                &:hover {
                    color: $color-blue;
                }
            }
        }

    }
}
</style>