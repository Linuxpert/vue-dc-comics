<template>
  <footer>
      <div class="info">
          <a  :href="info.urls" class="item" v-for="info, i in infos" :key="i">
              <img :src="info.img" :alt="info.text">
              <p>{{info.text}}</p>
          </a>
      </div>
      <div class="fMenu">
          <div class="links">
              <ul>
                  <h3>DC COMICS</h3>
                  <li v-for="link, i in dcComicsLinks" :key="i">
                      <a :href="link.urls">{{link.text}}</a>
                  </li>
              </ul>
              <ul>
                  <h3>SHOPS</h3>
                  <li v-for="link, i in shopLinks" :key="i">
                      <a :href="link.urls">{{link.text}}</a>
                  </li>
              </ul>
              <ul>
                  <h3>DC</h3>
                  <li v-for="link, i in DCLinks" :key="i">
                      <a :href="link.urls">{{link.text}}</a>
                  </li>
              </ul>
              <ul>
                  <h3>SITES</h3>
                  <li v-for="link, i in sitesLinks" :key="i">
                      <a :href="link.urls">{{link.text}}</a>
                  </li>
              </ul>
              <img src="../../public/assets/img/dc-logo-bg.png" alt="">
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
                  text: "DIGITAL COMICS",
                  urls: "#"
              },
              {
                  img: "assets/img/buy-comics-merchandise.png",
                  text: "DC MERCHANDISE",
                  urls: "#"
              },
              {
                  img: "assets/img/buy-comics-subscriptions.png",
                  text: "SUBSCRIPTION",
                  urls: "#"
              },
              {
                  img: "assets/img/buy-comics-shop-locator.png",
                  text: "COMIC SHOP LOCATOR",
                  urls: "#"
              },
              {
                  img: "assets/img/buy-dc-power-visa.svg",
                  text: "DC POWER VISA",
                  urls: "#"
              }
          ],
          dcComicsLinks: [
              {
                  text:"Characters",
                  urls:"#"
              },
              {
                  text:"Comics",
                  urls:"#"
              },
              {
                  text:"Movies",
                  urls:"#"
              },
              {
                  text:"Tv",
                  urls:"#"
              },
              {
                  text:"Games",
                  urls:"#"
              },
              {
                  text:"Videos",
                  urls:"#"
              },
              {
                  text:"News",
                  urls:"#"
              },
          ],
          shopLinks:[
              {
                  text:"Shop DC",
                  urls:"#"
              },
              {
                  text:"Shop DC Collectibles",
                  urls:"#"
              },
          ],
          DCLinks:[
              {
                  text:"Terms Of Use",
                  urls:"#"
              },
              {
                  text:"Privacy policy (New)",
                  urls:"#"
              },
              {
                  text:"Ad Choises",
                  urls:"#"
              },
              {
                  text:"Advertising",
                  urls:"#"
              },
              {
                  text:"Jobs",
                  urls:"#"
              },
              {
                  text:"Subscriptions",
                  urls:"#"
              },
              {
                  text:"Talent Workshop",
                  urls:"#"
              },
              {
                  text:"CPSC Certificates",
                  urls:"#"
              },
              {
                  text:"Ratings",
                  urls:"#"
              },
              {
                  text:"Shop Help",
                  urls:"#"
              },
              {
                  text:"Contact Us",
                  urls:"#"
              },
          ],
          sitesLinks:[
              {
                  text:"DC",
                  urls:"#"
              },
              {
                  text:"MAD Magazine",
                  urls:"#"
              },
              {
                  text:"DC Kids",
                  urls:"#"
              },
              {
                  text:"DC Universe",
                  urls:"#"
              },
              {
                  text:"DC Power Visa",
                  urls:"#"
              },
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
            margin: 50px;
            cursor: pointer;
            text-decoration: none;
            
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
    .fMenu{
        background-image: url("../../public/assets/img/footer-bg.jpg");
        background-size: cover;
        // height: 200px;
        .links{
            display: flex;
            margin-left: 10%;
            ul{
                list-style-type: none;
                margin: 20px;
            }
            li{
                margin: 10px 0;
            }
            a{
                text-decoration: none;
                color: grey;
                &:hover{
                    color: white;
                    cursor: pointer;
                }
            }
            img{
                margin: 0 150px;
                height: 400px;
                width: 600px;
                object-fit: none
            }
        }
    }

</style>