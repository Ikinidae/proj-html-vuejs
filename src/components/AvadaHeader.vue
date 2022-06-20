<template>
  <header>
    <!-- prima riga con logo e menu -->
    <div class="d-flex justify-content-between align-items-center">
      <div>
        <img src="../assets/avada-music-logo.png" alt="Logo Avada Music">
      </div>
      <div>
        <p id="nav_button" @click="showNav = true">
          <font-awesome-icon icon="fa-solid fa-bars" />
        </p>
      </div>
    </div>

    <div v-if="showNav" id="hamburger_menu" class="d-flex flex-column align-items-center">
      <p class="close_button" @click="showNav = false">
        X
      </p>
      <div id="nav_content">
        <a class="menu_voice" href="" v-for="(item, i) in menu" :key="i">
          <h3>{{ item.section }}</h3>
        </a>
      </div>
    </div>

    <!-- parte centrale -->
    <div id="jumbotron" class="d-flex flex-column align-items-center">
      <h1>Untold Stories</h1>
      <p>There is an untold story behind every favorite song</p>
      <div>
        <button class="red_button">LATEST ALBUM</button>
        <button class="white_button">LIVE DATES</button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AvadaHeader',
  data() {
    return {
      menu: [
        { section: "Home" },
        { section: "Meet The Band" },
        { section: "Live Dates" },
        { section: "Latest News" },
        { section: "Albums" },
        { section: "Fans" }
      ],
      showNav: false,
    }
  },
  methods: {
    change_showNav() {
      if (this.showNav == false) {
        this.showNav == true;
      } else {
        this.showNav == false;
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-image: url(../assets/home_slider.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 750px;
  padding: 20px;
  color: white;

  img {
    width: 250px;
  }

  #nav_button {
    text-decoration: none;
    color: white;
    cursor: pointer;
  }

  .fa-bars {
    font-size: 30px;
  }

  #hamburger_menu {
    position: absolute;
    z-index: 1;
    top: 0;
    left: 0;
    padding: 20px;
    width: 100%;
    height: 750px;
    background: #ea4a56;

    .close_button {
      position: absolute;
      top: 20px;
      right: 45px;
      text-decoration: none;
      color: white;
      cursor: pointer;
    }

    .menu_voice {
      text-decoration: none;
      color: white;
    }
  }

  #jumbotron {
    padding-top: 150px;

    h1 {
      font-weight: bolder;
      font-size: 100px;
    }

    p {
      font-style: italic;
      margin-bottom: 40px;
    }

    button {
      border: none;
      color: white;
      padding: 10px 25px;
      margin: 10px;
      font-size: 12px;
      font-weight: bold;
    }

    .red_button {
      background-color: #ea4a56;

      &:hover {
        background-color: white;
        color: black;
      }
    }

    .white_button {
      background: none;
      border: 1px solid white;

      &:hover {
        background-color: white;
        color: black;
      }
    }
  }
}
</style>