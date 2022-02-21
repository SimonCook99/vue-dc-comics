<template>
  <div id="app">
    <myHeader/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'

export default {
  name: 'App',
  components: {
    myHeader
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
