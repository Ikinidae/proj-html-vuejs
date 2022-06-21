<template>
  <footer>
    <div id="logo_menu" class="d-flex justify-content-between align-items-center">
      <div>
        <img src="../assets/logo_footer.png" alt="">
      </div>

      <div>
        <span v-for="(item, i) in menu" :key="i">{{ item.section }}</span>
      </div>
    </div>

    <div id="copyright_socials" class="d-flex justify-content-between align-items-center">
      <div class="d-flex">
        <span class="my_border">&copy; Copyright 2012 - 2020</span>
        <!-- <hr> -->
        <span class="my_border">AVADA THEME BY THEMEFUSION</span>
        <span class="my_border">ALL RIGHTS RESERVED</span>
        <span>POWERED BY WORDPRESS</span>
      </div>

      <div id="socials" class="d-flex justify-content-between">
        <div id="facebook">
          <font-awesome-icon class="icon" icon="fa-brands fa-facebook-f" />
        </div>
        <div id="twitter">
          <font-awesome-icon class="icon" icon="fa-brands fa-twitter" />
        </div>
        <div id="instagram">
          <font-awesome-icon class="icon" icon="fa-brands fa-instagram" />
        </div>
        <div id="youtube">
          <font-awesome-icon class="icon" icon="fa-brands fa-youtube" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AvadaFooter',
  data() {
    return {
      menu: [
        { section: "Home" },
        { section: "Meet The Band" },
        { section: "Live Dates" },
        { section: "Latest News" },
        { section: "Albums" },
        { section: "Fans" }
      ]
    }
  }
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

#copyright_socials {
  background-color: #252a33;
  padding: 30px;

  span {
    color: #aeaeaf;
    font-size: 11px;
    margin-top: 0;
    margin-bottom: 0;
    margin-right: 10px;
    padding-right: 10px;
  }

  .my_border {
    border-right: 1px solid #aeaeaf;
  }
}

#socials {
  color: #aeaeaf;

  div {
    background-color: #323844;
    margin: 10px;

    .icon {
      font-size: 13px;
    }
  }

  #twitter, #youtube {
    padding: 10px 15px;
    border-radius: 10%;
  }

  #facebook {
    padding: 10px 18px;
    border-radius: 10%;
  }

  #instagram {
    padding: 10px 17px;
    border-radius: 10%;
  }
}
</style>