<template>
  <div id="app">
     <Header></Header>
     <Home></Home>
  </div>
</template>

<script>
import Header from './components/bars/Header';
import Home from './components/page/Home';
export default {
  name: 'app',
   components: { Home, Header },
}
</script>

<style lang="scss">
   @import './assets/style.scss';
</style>