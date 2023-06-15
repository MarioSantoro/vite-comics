<template>
    <main class="content-black">
        <div class=" container">
            <h1> -- > Content goes here </h1>
        </div>
    </main>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

main.content-black {
    background-color: #1c1c1c;
    color: $colorFontWhite;
    padding: 2rem 0;
}
</style>