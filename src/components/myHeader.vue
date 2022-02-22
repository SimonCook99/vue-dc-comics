<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="dc-logo">

      <nav>
          <ul>
              <!--ciclo che scorre lungo la lista passata come parametro in App.vue-->
              <li v-for="(item,index) in lista" :key="index">{{item}}</li>
          </ul>
      </nav>
  </header>
</template>

<script>

export default {
  name: 'myHeader',

  props:["lista"]
  
}

</script>

<style lang="scss">
    header{
        width: 80%;
        margin: auto;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 30px;

        img {
            margin-right: 250px;
        }

        ul{
            display: flex;
        }

        li{
            padding: 15px;
            display: flex;
            align-items: center;
            border-bottom: 2px solid transparent;

            &:hover{
                color: #0282f9;
                border-bottom: 2px solid #0282f9;
                cursor: pointer;

            }
        }
    }

</style>
