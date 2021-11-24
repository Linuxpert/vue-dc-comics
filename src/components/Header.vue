<template>
  <header>
      <img src="assets/img/dc-logo.png" alt="">
      <nav>
          <ul>
              <li v-for="link, i in links" :key="i">
                  <a :href="link.urls" :class="link.here ? 'active' : '' ">{{link.text}}</a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          links: [
              {
                  text: "CHARACTERS",
                  urls: "#",
                  here: false,
              },
              {
                  text: "COMICS",
                  urls: "#",
                  here: true,
              },
              {
                  text: "MOVIES",
                  urls: "#",
                  here: false,
              },
              {
                  text: "TV",
                  urls: "#",
                  here: false,
              },
              {
                  text: "GAMES",
                  urls: "#",
                  here: false,
              },
              {
                  text: "COLLECTIBLES",
                  urls: "#",
                  here: false,
              },
              {
                  text: "VIDEOS",
                  urls: "#",
                  here: false,
              },
              {
                  text: "FANS",
                  urls: "#",
                  here: false,
              },
              {
                  text: "NEWS",
                  urls: "#",
                  here: false,
              },
              {
                  text: "SHOP",
                  urls: "#",
                  here: false,
              },
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    header{
        display: flex;
        justify-content: space-around;
        align-items: center;

        li {
            display: inline-block;
            margin: 20px;

            a {
                color: #000;
                text-decoration: none;
                font-size: 15px;
                &.active{
                    color: blue;
                    padding-bottom: 47px;
                    border-bottom: 6px solid blue;
                }
                &:hover{
                    color: blue;
                    cursor: pointer;
                }
            }
        }
    }
</style>