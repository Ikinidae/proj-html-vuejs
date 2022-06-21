<template>
  <div>
    <section id="quote">
      <p>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're good. And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to."</p>
      <a href="" id="play_button">
        <font-awesome-icon id="font_awesome_play" icon="fa-solid fa-circle-play" />
      </a>
    </section>
  </div>
</template>

<script>
export default {
  name: 'AvadaFooter',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#quote {
  background-image: url(../assets/home-testimonial-parallax.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 600px;
  color: white;
  text-align: center;
  padding: 200px 400px 300px 400px;
  font-style: italic;
  font-size: 20px;

  #play_button {
    color: #eb4b54;
    font-size: 50px;
    text-decoration: none;

    #font_awesome_play {
      border-radius: 100%;
      background-color: white;
    }
  }
}
</style>