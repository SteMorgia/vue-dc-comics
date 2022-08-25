<template>
  <div id="app">
    <MyHeader/>
    <MyJumbo/>
    <MyBody/>
    <MyInfo/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyBody from './components/MyBody';
import MyFooter from './components/MyFooter';
import MyInfo from './components/MyInfo';
import MyJumbo from './components/MyJumbo'



export default {
  name: 'App',
  components: {
    MyHeader,
    MyBody,
    MyFooter,
    MyInfo,
    MyJumbo,
    
}
}
</script>

<style lang="scss">
  @import './styles/general.scss';
  @import './styles/vars.scss';
</style>
