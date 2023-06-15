<script>
import AppHeader from './components/AppHeader.vue';

export default {
  data() {
    return {
      components: {
        AppHeader,
      }
    };
  },
  components: { AppHeader }
}
</script>

<template>
  <AppHeader />
</template>

<style lang="scss">
@import "./styles/general.scss";
</style>
