<template>
  <div id="app">
     <Header></Header>
  </div>
</template>

<script>
import Header from './components/bars/Header';
export default {
  name: 'app',
   components: { Header },
}
</script>

<style lang="scss">
   @import './assets/style.scss';
</style>