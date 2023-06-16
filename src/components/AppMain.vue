<template>
    <main>
        <section>
            <div class="jumbo">
                <img src="../assets/img/jumbotron.jpg" alt="Jumbo image">
                <div class="series">
                    <p>Current Series</p>
                </div>
            </div>
            <div class="content-black">
                <div class=" container">
                    <AppCards v-for="card in listCards" :cards="card" />
                </div>
            </div>
        </section>
        <section>
            <div class="content-blue">
                <AppSectionBlue />
            </div>
        </section>
    </main>
</template>
<script>
import AppSectionBlue from './AppSectionBlue.vue';
import AppCards from './AppCards.vue';
export default {
    data() {
        return {
            listCards: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5ddbc1qk55vk7wjgzg3pmxlh59rv5dlgewd9jem5nrt4w/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    },

    components: {
        AppSectionBlue,
        AppCards,
    }
}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;


div.jumbo {
    position: relative;

    img {
        height: 450px;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }

    div.series {
        background-color: $colorFontBlue;
        padding: .55rem 1.44rem;
        position: absolute;

        left: 20%;
        bottom: -15px;

        p {
            text-transform: uppercase;
            color: $colorFontWhite;
            font-weight: bold;
            font-size: 1.2rem;
        }
    }
}

div.content-black {
    background-color: #1c1c1c;
    color: $colorFontWhite;
    padding: 2.5rem 0;
}

div.content-blue {
    background-color: $colorFontBlue;
    padding: 3rem 0;
}
</style>