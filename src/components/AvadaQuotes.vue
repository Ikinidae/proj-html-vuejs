<template>
  <div>
    <section id="quote">
      <p>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're good. And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to."</p>
      <img src="../assets/band_interview_play_icon.png" alt="">
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

  img {
    width: 60px;
  }
}
</style>