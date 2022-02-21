<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="dc-logo">

      <nav>
          <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>Tv</li>
              <li>Games</li>
              <li>Collectibles</li>
              <li>Videos</li>
              <li>Fans</li>
              <li>News</li>
              <li>Shop</li>
          </ul>
      </nav>
  </header>
</template>

<script>

export default {
  name: 'myHeader',
  
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
