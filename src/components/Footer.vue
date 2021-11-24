<template>
  <footer>
      <div class="info">
          <div class="item" v-for="info, i in infos" :key="i">
              <img :src="info.img" :alt="info.text">
              <p>{{info.text}}</p>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data(){
      return{
          infos: [
              {
                  img: "assets/img/buy-comics-digital-comics.png",
                  text: "DIGITAL COMICS"
              },
              {
                  img: "assets/img/buy-comics-merchandise.png",
                  text: "DC MERCHANDISE"
              },
              {
                  img: "assets/img/buy-comics-subscriptions.png",
                  text: "SUBSCRIPTION"
              },
              {
                  img: "assets/img/buy-comics-shop-locator.png",
                  text: "COMIC SHOP LOCATOR"
              },
              {
                  img: "assets/img/buy-dc-power-visa.svg",
                  text: "DC POWER VISA"
              }
          ]
      }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .info{
        background-color: rgb(0, 70, 199);
        height: 150px;
        display: flex;
        align-items: center;
        justify-content: center;
        .item{
            display: flex;
            justify-self: center;
            align-items: center;
            margin: 20px;
            
            img{
                width: 55px;
            }
            p{
                color: white;
                margin: 10px;
                font-size: 14px;
            }
        }
    }
</style>