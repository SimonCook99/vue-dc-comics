<template>
  <div id="app">

    <!--Passo la listaHeader al componente header come prop-->
    <myHeader 
      :lista="listaHeader"
    />

    <myJumbotron/>
    <mainContent/>
    <buySection/>

    <!--Passo le listeFooter al componente footer come props-->
    <myFooter 
      :lista1="listeFooter.lista1" 
      :lista2="listeFooter.lista2" 
      :lista3="listeFooter.lista3"
      :lista4="listeFooter.lista4"
    />

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
    //Qui ci sarà l'insieme di liste da creare dinamicamente nei vari componenti
    return{

      listaHeader: ["Characters", "Comics", "Movies", "Tv", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"],

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
