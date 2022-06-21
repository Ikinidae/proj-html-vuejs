<template>
  <div>
    <section id="music_is_life" class="d-flex justify-content-center">
      <div class="d-flex flex-column align-items-center section_width">
        <!-- MANCA LINEA ROSSA IN ALTO -->
        <!-- <hr id="red_line"> -->
        <h1>{{title}}</h1>
        <hr>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur deserunt odit velit ad repellat soluta
          reiciendis accusamus maxime quam aliquam? Quibusdam, inventore. Facilis vitae vero iure laborum
          necessitatibus? Id, fugiat?</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'MusicIsLife',
  props: {
    title: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.section_width {
  width: 40%;
}

#music_is_life {
  height: auto;
  padding-top: 60px;
  padding-bottom: 50px;
  // border-top: 5px solid #eb4b54;

  // #red_line {
  //   border-top: 5px solid #eb4b54;
  //   width: 200px;
  //   position: absolute;
  //   top: 0;
  // }

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
  }
}
</style>