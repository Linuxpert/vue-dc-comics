<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="">
      <nav>
          <ul>
              <li>
                  <a href="#">CHARACTERS</a>
              </li>

              <li>
                  <a href="#" class="active"> COMICS</a>
              </li>

              <li>
                  <a href="#">MOVIES</a>
              </li>

              <li>
                  <a href="#">TV</a>
              </li>

              <li>
                  <a href="#">GAMES</a>
              </li>

              <li>
                  <a href="#">COLLECTIBLES</a>
              </li>

              <li>
                  <a href="#">VIDEOS</a>
              </li>

              <li>
                  <a href="#">FANS</a>
              </li>

              <li>
                  <a href="#">NEWS</a>
              </li>

              <li>
                  <a href="#">SHOP</a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  
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
                }
            }
        }
    }
</style>