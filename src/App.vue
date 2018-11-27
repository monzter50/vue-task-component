<template>
  <div id="app">
    <div class="grid-container">
        <Header/>      
        <Aside :list="list"/>
        <Main/>
        <Footer msg="Welcome to Your Vue.js App"/>
    </div>
      
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import Aside from './components/Aside';
import Main from './components/Main';
import Header from './components/Header';

export default {
  name: 'app',
  components: {
    Footer,
    Aside,
    Main,
    Header
  },
     data:function () {
        return {
            list:[
                "Item 1",
                "Item 2",
                "Item 3",
                "Item 4",
                "Item 5",
            ]
        }
    }
}
</script>

<style lng="scss">
@import './scss/_styles.scss';
</style>
