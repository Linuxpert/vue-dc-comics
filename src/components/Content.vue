<template>
  <main>
    <Jumbo/>
  </main>
</template>

<script>
import Jumbo from '@/components/Jumbo.vue'
export default {
  name: "Content",
  components: {
    Jumbo
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {

    background-color: rgb(63, 63, 63);
    // height: 150px;
    display: flex;
    align-items: center;
    margin-top: 10px;
  

    h1 {
        color: white;
        margin-left: 10%;
    }
  
}
</style>