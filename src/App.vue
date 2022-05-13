<template>

  <section>

    <header-component />

  </section>

</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'


export default {
  name: 'App',
  components: {
    HeaderComponent
  }
}
</script>

<style lang="scss">

@import "./assets/style/variable.scss";
@import "./assets/style/global.scss";
@import "./assets/style/utils.scss";


</style>
