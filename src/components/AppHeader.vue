<template>
    <header class="container flex">
        <div class="image-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav id="top-navbar">
            <ul>
                <li>Characters</li>
            </ul>
        </nav>
    </header>
</template>
<script>

export default {

}
</script>
<style lang="scss">
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

header {
    padding: 1rem 0;

    div.image-logo img {
        width: 80px;
        height: 80px;
    }
}
</style>