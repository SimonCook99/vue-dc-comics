<template>
  <section>

      <ul>
          <li>
              <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
              <p>digital comics</p>
          </li>
          <li>
              <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
              <p>DC merchandise</p>
          </li>
          <li>
              <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
              <p>Subscription</p>
          </li>
          <li>
              <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator">
              <p>comic shop locator</p>
          </li>
          <li>
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              <p>DC power visa</p>
          </li>
      </ul>

  </section>
</template>

<script>

export default {
  name: 'buySection',
  
}

</script>

<style lang="scss">
    section{
       background-color: #0282f9;

        ul{
            display: flex;
            justify-content: center;
        }

        li{
            display: flex;
            align-items: center;
            padding: 30px;

            img{
                max-width: 40px;
                margin-right: 15px;
            }
            p{
                text-transform: uppercase;
                color: white;
            }
        }
    }
    
</style>



