<script>
export default {
    name: 'MainCard',
    props: {
        card: Object
    }
};
</script>
<template>
    <div class="card">
        <img :src="card.thumb" alt="card.type">
        <h3>{{ card.series }}</h3>
    </div>
</template>
<style scoped lang="scss">
.card {
    flex-basis: calc(100% / 6);
}

img {
    display: block;

}

h3 {
    color: white;
    padding-right: 2px;
}
</style>