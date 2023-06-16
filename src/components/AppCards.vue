<template>
    <div class="card ">
        <img :src="cards.thumb" alt="">
        <h3>{{ cards.series }}</h3>
    </div>
</template>
<script>
export default {
    props: {
        cards: Object,
    }
}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

div.card {
    width: calc(100% / 6 - 25px);

    margin-right: 25px;
    margin-bottom: 1rem;

    img {
        width: 100%;
        height: 175px;
        margin-bottom: .55rem
    }

    ;
}
</style>