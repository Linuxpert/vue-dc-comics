<template>
  <div class="comic">
    <img :src="details.thumb" :alt="details.series" />
    <h4>{{ details.series }}</h4>
    <p>{{ details.type }}</p>
    <p>{{ details.price }}</p>
  </div>
</template>

<script>
export default {
  name: "Comics",
  props: {
    details: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.comic {
  width: calc(100% / 6);
  margin-bottom: 60px;
  text-decoration: none;

  h4 {
    color: #fff;
  }
  p {
    color: #fff;
  }
}

</style>