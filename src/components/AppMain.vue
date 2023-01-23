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
        <div>
            <section class="content">
                <MainCard v-for="card in cards" :key="card.series" :card="card"></MainCard>
                <button> LOAD MORE </button>
            </section>
        </div>
        <section></section>
    </main>
</template>

<style scoped lang="scss">
@use '../assets/scss/colors.scss' as *;
@use '../assets/scss/mixin.scss' as *;


button {
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

div {
    background-color: $color-black;
    width: 100%;

    .content {
        @include container;
        min-height: 100px;
        display: flex;
        flex-wrap: wrap;
        padding-top: 20px;
        padding-bottom: 60px;



        h1 {
            padding-top: 30px;
            color: $color-white;
        }

    }

}
</style>