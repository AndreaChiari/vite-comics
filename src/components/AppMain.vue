<script>

import MainCard from './MainCard.vue'

export default {
    name: 'Main',
    components: { MainCard },
    props: {
        cards: Array
    }
}
</script>

<template>
    <main>
        <div class="jumbotron">
            <button class="jumbo-button"> CURRENT SERIES</button>
        </div>
        <div class="card-container">
            <section class="content">
                <MainCard v-for="card in cards" :key="card.series" :card="card"></MainCard>
                <button class="button-cards"> LOAD MORE </button>
            </section>
        </div>
        <section></section>
    </main>
</template>


<style scoped lang="scss">
@use '../assets/scss/colors.scss' as *;
@use '../assets/scss/mixin.scss' as *;

.jumbotron {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    position: relative;

    .jumbo-button {
        border: 1px solid $color-blue;
        padding: 5px 40px;
        background-color: $color-blue;
        color: $color-white;
        cursor: pointer;
        position: absolute;
        font-size: 150%;
        bottom: -20px;
        left: 17%;
    }

}

.button-cards {
    border: 1px solid $color-blue;
    padding: 5px 40px;
    background-color: $color-blue;
    color: $color-white;
    cursor: pointer;
    position: absolute;
    bottom: 2%;
    left: 50%;
    transform: translate(-50%);
}

main {
    position: relative;
    z-index: 2;

}

.card-container {
    background-color: $color-black;
    width: 100%;

    .content {
        @include container;
        min-height: 100px;
        display: flex;
        flex-wrap: wrap;
        padding-top: 50px;
        padding-bottom: 60px;



        h1 {
            padding-top: 30px;
            color: $color-white;
        }

    }

}
</style>