<template>
  <header>
    <!-- prima riga con logo e menu -->
    <div class="d-flex justify-content-between align-items-center">
      <div>
        <img src="../assets/avada-music-logo.png" alt="Logo Avada Music">
      </div>
      <div>
        <font-awesome-icon icon="fa-solid fa-bars" />
      </div>
    </div>

    <!-- <div id="hamburger_menu">
      <h3>Home</h3>
      <h3>Meet The Band</h3>
      <h3>Live Dates</h3>
      <h3>Latest News</h3>
      <h3>Albums</h3>
      <h3>Fans</h3>
    </div> -->

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
      menu: ["Home", "Meet The Band", "Live Dates", "Latest News", "Albums", "Fans"]
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

  .fa-bars {
    font-size: 30px;
  }

  #hamburger-menu {
    position: absolute;
    top: 0;
    left: 0;
    display: none;
    padding: 20px;
    width: 100%;
    height: 100%;
    background: #ea4a56;

    .active {
      display: block;
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
      background:none;
      border: 1px solid white;

      &:hover {
        background-color: white;
        color: black;
      }
    }
  }
}
</style>