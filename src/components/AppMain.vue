<template>
    <main>
        <section>
            <div class="content-black">
                <div class=" container">
                    <h1> -- > Content goes here </h1>
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
export default {
    data() {
        return {

        }
    },

    components: {
        AppSectionBlue,
    }
}
</script>
<style lang="scss" scoped>
@use "../styles/utilities/mixins.scss" as *;
@use "../styles/utilities/variables.scss" as *;

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