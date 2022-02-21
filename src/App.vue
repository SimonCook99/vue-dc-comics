<template>
  <div id="app">
    <myHeader/>
    <mainContent/>
    <buySection/>
    <myFooter/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import mainContent from './components/mainContent.vue'
import buySection from './components/buySection.vue'
import myFooter from './components/myFooter.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    mainContent,
    buySection,
    myFooter
  }
}
</script>

<style lang="scss">

  @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body{
    font-family: 'Roboto', sans-serif;
  }

</style>
