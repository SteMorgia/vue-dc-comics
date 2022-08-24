<template>
  <div id="app">
    <MyHeader/>
    <MyBody/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyBody from './components/MyBody';
import MyFooter from './components/MyFooter'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyBody,
    MyFooter
}
}
</script>

<style lang="scss">
  @import './styles/general.scss';
  @import './styles/vars.scss';
</style>
