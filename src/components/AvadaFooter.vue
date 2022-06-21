<template>
  <footer>
    <div id="logo_menu" class="d-flex justify-content-between align-items-center">
      <div>
        <img src="../assets/logo_footer.png" alt="">
      </div>

      <div>
        <span>Home</span>
        <span>Meet The Band</span>
        <span>Live Dates</span>
        <span>Latest News</span>
        <span>Albums</span>
        <span>Fans</span>
      </div>
    </div>
    <h1>Footer</h1>
  </footer>
</template>

<script>
export default {
  name: 'AvadaFooter',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#logo_menu {
  background-color: #323844;
  padding: 40px 30px;

  img {
    width: 170px;
  }

  span {
    color: #aeaeaf;
    font-size: 11px;
    margin: 10px;
  }
}
</style>