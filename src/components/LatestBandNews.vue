<template>
  <section id="news" class="d-flex flex-column align-items-center">
    <MusicIsLife class="music_is_life" title="Latest Band News" />

    <!-- news -->
    <b-container>
      <b-row>
        <b-col cols="2">1</b-col>

        <!-- news sx -->
        <b-col id="news_sx" cols="5">
          <!-- notizia orizzontale -->
          <div class="single_new">
            <div class="img_container horizontal_img_container">
              <img src="../assets/blog_music_techo-800x400.jpg" alt="">
            </div>
            <div class="text_container">
              <h5>Technology and music</h5>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
            </div>
          </div>

          <!-- blocco due notizie verticali -->
          <b-row>
            <b-col>
              <div class="single_new">
                <div class="img_container vertical_img_container">
                  <img class="vertical_img" src="../assets/blog-post3-600x900.jpg" alt="">
                </div>
                <div class="text_container">
                  <h5>While my guitar gently weeps</h5>
                  <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
                </div>
              </div>
            </b-col>

            <b-col>
              <div class="single_new">
                <div class="img_container vertical_img_container">
                  <img class="vertical_img" src="../assets/blog-post4-600x900.jpg" alt="">
                </div>
                <div class="text_container">
                  <h5>It just sounds better</h5>
                  <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
                </div>
              </div>
            </b-col>
          </b-row>

          <!-- notizia orizzontale -->
          <div class="single_new">
            <div class="img_container horizontal_img_container">
              <img src="../assets/blog_flavor_rock-800x400.jpg" alt="">
            </div>
            <div class="text_container">
              <h5>The flavor of rock</h5>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
            </div>
          </div>
        </b-col>

        <!-- news dx -->
        <b-col cols="3">
          <div class="single_new">
            <div class="img_container vertical_img_container">
              <img class="vertical_img" src="../assets/blog-post1-600x900.jpg" alt="">
            </div>
            <div class="text_container">
              <h5>Taking it back to the old school</h5>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
            </div>
          </div>

          <div class="single_new">
            <div class="img_container vertical_img_container">
              <img class="vertical_img" src="../assets/blog-post2-600x900.jpg" alt="">
            </div>
            <div class="text_container">
              <h5>Sharing the stage with a legend</h5>
              <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. At omnis similique labore?</p>
            </div>
          </div>
        </b-col>
        <b-col cols="2">1</b-col>
      </b-row>
    </b-container>

    <p id="all_latest_news">
      VIEW ALL LATEST NEWS
    </p>
  </section>
</template>

<script>
import MusicIsLife from './MusicIsLife.vue';

export default {
  name: 'LatestBandNews',
  components: {
    MusicIsLife
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.section_width {
  width: 40%;
}

#news {
  height: auto;
  background-color: #252a33;

  .music_is_life {
    width: 100%;
  }

  h1 {
    color: white;
    font-size: 40px;
    font-weight: bolder;
    margin-bottom: 0;
  }

  hr {
    border-top: #aeaeaf solid 1px;
    width: 140px;
    margin-bottom: 30px;
  }

  p {
    color: #aeaeaf;
    font-size: 13px;
    margin-bottom: 50px;
  }

  .single_new {
    background-color: #323844;
    margin-bottom: 25px;

    .horizontal_img_container {
      height: 150px;
    }

    .vertical_img_container {
      height: 400px;

      .vertical_img {
        height: 100%;
      }
    }

    .img_container {
      width: 100%;
      overflow: hidden;

      img {
        width: 100%;
      }
    }

    .text_container {
      padding: 15px 20px;

      h5 {
        color: #eb4b54;
        font-weight: bolder;
        font-size: 15px;
      }

      p {
        margin: 0;
      }
    }
  }

  #all_latest_news {
    background-color: #eb4b54;
    width: 100%;
    text-align: center;
    margin-top: 30px;
    padding-top: 30px;
    padding-bottom: 30px;
    color: white;
    font-size: 12px;
    font-weight: bolder;
    cursor: pointer;

    &:hover {
      color: black;
      background-color: white;
    }
  }
}
</style>