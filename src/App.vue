<template>
  <div id="app">
    <MyHeader/>
    <MyBody/>
    <MyInfo/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyBody from './components/MyBody';
import MyFooter from './components/MyFooter';
import MyInfo from './components/MyInfo'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyBody,
    MyFooter,
    MyInfo
}
}
</script>

<style lang="scss">
  @import './styles/general.scss';
  @import './styles/vars.scss';
</style>
