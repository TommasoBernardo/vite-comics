<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>



<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
  </div>
</template>



<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
li{
  list-style-type: none;
}
.color-grey{
  text-decoration: none;
  color: lightgray;
}

.color-list{
  text-decoration: none;
  color: black;
}
</style>