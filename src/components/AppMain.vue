<script>
export default {
    name: 'Main'
}
</script>

<template>
    <main>
        <div>
            <section class="content">
                <h1> -->Content goes here </h1>
            </section>
        </div>
        <section></section>
    </main>
</template>

<style scoped lang="scss">
@use '../assets/scss/colors.scss' as *;
@use '../assets/scss/mixin.scss' as *;

div {
    background-color: $color-black;
    width: 100%;

    .content {
        @include container;
        height: 100px;



        h1 {

            padding-top: 30px;
            color: $color-white;
        }
    }

}
</style>