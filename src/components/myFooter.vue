<template>
  <footer>
      <!-- Footer principale che include le liste e la sezione social (in un altro componente)-->
      <div class="footer-list">
            <div class="first-section">
                <h2>DC comics</h2>

                <ul>
                    <!--ciclo che scorre lungo la lista passata come parametro in App.vue-->
                    <li v-for="(lista, index) in lista1" :key="index">{{lista}}</li>
                </ul>

                <h2>Shop</h2>

                <ul>
                    <li v-for="(lista, index) in lista2" :key="index">{{lista}}</li>
                </ul>
            </div>

            <div class="second-section">
                <h2>DC</h2>

                <ul>
                    <li v-for="(lista, index) in lista3" :key="index">{{lista}}</li>
                </ul>

            </div>

            <div class="third-section">
                <h2>Sites</h2>

                <ul>
                    <li v-for="(lista,index) in lista4" :key="index">{{lista}}</li>
                </ul>
            </div>

            <img src="../assets/img/dc-logo-bg.png" alt="logo bg">    
       </div>

        <!--Chiamo e importo il componente finale del footer-->
        <finalFooter/>
  </footer>
</template>

<script>

import finalFooter from "./finalFooter.vue"

export default {
  name: 'mainContent',
  components: {
    finalFooter
  },
  props:["lista1", "lista2", "lista3", "lista4"]
  
}

</script>

<style lang="scss">
    .footer-list{
        background-image: url("../assets/img/footer-bg.jpg");
        display: flex;
        justify-content: center;
        padding: 30px;
        height: 450px;
        overflow: hidden;

        img{
            margin-left: 200px;
            height: 550px;
            margin-left: 200px;
            overflow: hidden;
            position: relative;
            bottom: 90px;
        }

        h2{
            color: white;
            margin-left: 10px;
        }

        ul{
            margin-right: 20px;
        }

        li{
            color: grey;
            list-style: none;
            margin: 10px;
        }
    }

    
</style>



