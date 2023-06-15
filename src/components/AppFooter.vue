<template>
    <footer>
        <div class="footer-upper">
            <div class="container flex">
                <div class="comics-shop">
                    <ul>
                        <li>
                            <h1>DC Comics</h1>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <ul>
                        <li>
                            <h1>Shop</h1>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>

                <ul>
                    <li>
                        <h1>DC</h1>
                    </li>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
                <ul>
                    <li>
                        <h1>SITES</h1>
                    </li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
        <div class="footer-lower">
            <div class="container flex between">
                <div class="signUp">
                    <p>Sign-up now!</p>
                </div>
                <div class="social-icons">
                    <ul>
                        <li>BBBB</li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

footer {
    div.footer-upper {
        position: relative;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        padding: 2rem 0;
        overflow: hidden;


        ul {
            margin-right: 2rem;

            li {
                color: gray;
                line-height: 30px;
                font-size: .88rem;

                h1 {
                    color: $colorFontWhite;
                    margin-bottom: 1rem;
                    font-size: 1.3rem;
                    text-transform: uppercase;
                }
            }
        }

        div.comics-shop ul:nth-child(1) {
            margin-bottom: 2rem;
        }

        img {
            width: 620px;
            position: absolute;
            top: -70px;
            left: 55%;
        }
    }

}

div.footer-lower {
    background-color: #303030;
    padding: 2rem 0;

    div.signUp {
        border: 1px solid $colorFontBlue;
        padding: .88rem 1rem;
        text-transform: uppercase;
        font-weight: bold;

        p {
            color: $colorFontWhite;
        }
    }

}
</style>