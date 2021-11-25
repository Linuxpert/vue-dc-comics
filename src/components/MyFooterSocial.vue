<template>
  <footer>
      <div class="signUp">
          <span>SIGN-UP NOW!</span>
      </div>
      <div class="social">
          <span>FOLLOW US</span>
          <i class="fab fa-facebook"></i>
          <i class="fab fa-twitter-square"></i>
          <i class="fab fa-youtube"></i>
          <i class="fab fa-pinterest"></i>
      </div>
  </footer>
</template>

<script>
export default {
  name: "MyFooterSocial",
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer{
        background-color: rgb(53, 52, 52);
        height: 70px;
        display: flex;
        align-items: center;
        justify-content: space-around;
        .signUp{

            span{
                padding: 10px;
                border: 2px solid rgb(0, 70, 199);
                color: white;
                cursor: pointer;
            }
        }
        
        .social{
            span{
                color: rgb(0, 70, 199) ;
            }
            
        }
    }

</style>