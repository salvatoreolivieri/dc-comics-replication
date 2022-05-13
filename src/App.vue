<template>

  <section>

    <header-component />

    <main-component />

    <BlueBar />

    <FooterComponent />

  </section>

</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import BlueBar from './components/BlueBar.vue'
import FooterComponent from './components/FooterComponent.vue'


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueBar,
    FooterComponent
}
}
</script>

<style lang="scss">

@import "./assets/style/variable.scss";
@import "./assets/style/global.scss";
@import "./assets/style/utils.scss";


</style>
