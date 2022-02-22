<template>
  <div id="app">
    <myHeader/>
    <myJumbotron/>
    <mainContent/>
    <buySection/>
    <myFooter :lista1="lista1" :lista2="lista2" :lista3="lista3"/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myJumbotron from './components/myJumbotron.vue'
import mainContent from './components/mainContent.vue'
import buySection from './components/buySection.vue'
import myFooter from './components/myFooter.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    myJumbotron,
    mainContent,
    buySection,
    myFooter
  },

  data(){
    return{
      listeFooter: {
        lista1: ["Characters", "Comics", "Movies", "Tv", "Games", "Videos", "News"],
        lista2: ["Shop DC", "Shop DC Collectibles"],
        lista3: ["Terms of use", "Privacy policy (New)","Ad Choices","Advertising","Jobs","Subscriptions","Talent workshops","CPSC certificates","Ratings","Shop helps","contact us"],
        lista4: ["DC", "Mad Magazine", "DC Kids", "DC Universe", "DC Power visa"]
      }
    }
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
