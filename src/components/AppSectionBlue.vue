<template>
    <div class="container">
        <ul class="flex between">
            <li v-for="item in listMerch" class="flex centered-flex">
                <img :src="getImagePath(item.image)" alt="Image merch">
                <p>{{ item.text }}</p>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    data() {
        return {
            listMerch: [
                {
                    image: "../src/assets/img/buy-comics-digital-comics.png",
                    text: "Digital Comics"
                },
                {
                    image: "../src/assets/img/buy-comics-merchandise.png",
                    text: "Dc merchandise"
                },
                {
                    image: "../src/assets/img/buy-comics-subscriptions.png",
                    text: "subscriptions"
                },
                {
                    image: "../src/assets/img/buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    image: "../src/assets/img/buy-dc-power-visa.svg",
                    text: "dc power visa"
                },
            ]
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        },
    }
}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

li {
    img {
        width: 55px;
        height: 55px;
        object-fit: contain;
    }

    p {
        color: $colorFontWhite;
        text-transform: uppercase;
        margin-left: 1rem;
    }

}
</style>