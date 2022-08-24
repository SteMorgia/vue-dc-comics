<template>
  <div id="app">
    <MyHeader/>
    <MyBody/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyBody from './components/MyBody';


export default {
  name: 'App',
  components: {
    MyHeader,
    MyBody,

    
}
}
</script>

<style lang="scss">
  @import './styles/general.scss';
  @import './styles/vars.scss';
</style>
