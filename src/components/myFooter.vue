<template>
  <footer>
      <div class="footer-list">
            <div class="first-section">
                <h2>DC comics</h2>

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

                <h2>Shop</h2>

                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC collectibles</li>
                </ul>
            </div>

            <div class="second-section">
                <h2>DC</h2>

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
                    <li>Collectibles</li>
                </ul>

            </div>

            <div class="third-section">
                <h2>Sites</h2>

                <ul>
                    <li>DC</li>
                    <li>Mad Magazine</li>
                    <li>DC kids</li>
                    <li>DC universe</li>
                    <li>DC power visa</li>
                </ul>
            </div>

            <img src="../assets/img/dc-logo-bg.png" alt="logo bg">    
        </div>

        <finalFooter/>
  </footer>
</template>

<script>

import finalFooter from "./finalFooter.vue"

export default {
  name: 'mainContent',
  components: {
      finalFooter
  }
  
}

</script>

<style lang="scss">
    .footer-list{
        background-image: url("../assets/img/footer-bg.jpg");
        display: flex;
        justify-content: center;
        padding: 30px;
        height: 450px;

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



