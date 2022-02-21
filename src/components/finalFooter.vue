<template>
    <footer>
      
      <div class="signup">
          <button>Sign-up Now</button>
      </div>

      <div class="social">
          <h2>Follow us</h2>
          <img src="../assets/img/footer-facebook.png" alt="facebook">
          <img src="../assets/img/footer-twitter.png" alt="facebook">
          <img src="../assets/img/footer-youtube.png" alt="facebook">
          <img src="../assets/img/footer-pinterest.png" alt="facebook">
          <img src="../assets/img/footer-periscope.png" alt="facebook">
      </div>
      
    </footer>
</template>

<script>

export default {
  name: 'finalFooter',
  
}

</script>

<style scoped lang="scss">
    footer{
       background-color: #303030;
       display: flex;
       justify-content: space-around;
       align-items: center;
       padding: 40px;
       height: 120px;

        h2{
           color: white;
        }

        button{
            padding: 20px;
            background: none;
            border: 1px solid #0282f9;
            color: white;
            text-transform: uppercase;
        }

       .social{
           display: flex;
           align-items: center;

           h2, img{
               margin-right: 20px;
           }

           h2{
               color: #2d4ac5;
           }
           
       }
   }
</style>



