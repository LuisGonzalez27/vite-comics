<template>
  <HeaderComponent />
  <main>
    <JumbotronComponent />
    <MainComponent />
  </main>
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponet.vue';
import JumbotronComponent from './components/JumbotronComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';


export default {
  components: {
    HeaderComponent,
    JumbotronComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss" scoped>

</style>