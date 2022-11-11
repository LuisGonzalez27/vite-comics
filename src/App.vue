<template>
  <HeaderComponent />
  <main>
    <MainComponent />
    <ContentComponent />
  </main>
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponet.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import ContentComponent from './components/ContentComponent.vue';

export default {
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    ContentComponent,
  }
}
</script>

<style lang="scss" scoped>

</style>