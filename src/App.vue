<template>

  <section>

    <header-component />

    <main-component />

    <BlueBar />

  </section>

</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import BlueBar from './components/BlueBar.vue'


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    BlueBar
}
}
</script>

<style lang="scss">

@import "./assets/style/variable.scss";
@import "./assets/style/global.scss";
@import "./assets/style/utils.scss";


</style>
