<template>
    <header>
        <div class="container flex between centered-flex">
            <div class="image-logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav id="top-navbar">
                <ul class="flex ">
                    <li v-for="(navItem, index) in navBarTop">
                        <a :class="navItem.active ? 'active' : 'non-active'" :href="navItem.link"
                            @click="changeActive(index)">{{ navItem.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>

export default {
    data() {
        return {
            navBarTop: [
                {
                    link: "#",
                    text: "Characters",
                    active: false,
                },
                {
                    link: "#",
                    text: "Comics",
                    active: true,
                },
                {
                    link: "#",
                    text: "Movies",
                    active: false,
                },
                {
                    link: "#",
                    text: "TV",
                    active: false,
                },
                {
                    link: "#",
                    text: "games",
                    active: false,
                },
                {
                    link: "#",
                    text: "collectibles",
                    active: false,
                },
                {
                    link: "#",
                    text: "videos",
                    active: false,
                },
                {
                    link: "#",
                    text: "fans",
                    active: false,
                },
                {
                    link: "#",
                    text: "news",
                    active: false,
                },
                {
                    link: "#",
                    text: "shop",
                    active: false,
                },
            ]
        }
    },

    methods: {
        changeActive(index) {
            for (let i = 0; i < this.navBarTop.length; i++) {
                this.navBarTop[i].active = false;
            }
            this.navBarTop[index].active = true;
        }
    }
}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

header {
    padding: 1rem 0;
    background-color: #fff;

    div.image-logo img {
        width: 80px;
        height: 80px;
    }

    ul li {
        margin-left: 2rem;
        font-weight: bold;

        a {
            padding: 2.8rem 0;
            color: black;
            text-decoration: none;
            text-transform: uppercase;
            font-size: .88rem;
        }
    }
}
</style>