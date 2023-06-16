<template>
    <div class="card ">
        <img :src="cards.thumb" alt="">
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
    width: calc(100% / 6 - 30px);

    margin-right: 30px;

    img {
        width: 100%;
        height: 170px;
    }

    ;
}
</style>