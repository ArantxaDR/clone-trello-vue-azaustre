<template>
  <app-header />
  <RouterView class="container" />
  <app-footer />
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style scoped>
.container {
  padding-bottom: 4rem;
}
</style>
