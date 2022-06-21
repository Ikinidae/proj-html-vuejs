<template>
  <main>
    <div id="music_is_life">
      <MusicIsLife title="Music Is Life"/>
    </div>

    <LatestBandNews/>

    <AvadaQuotes/>

    <LiveDates/>
  </main>
</template>

<script>
import MusicIsLife from './MusicIsLife.vue';
import LatestBandNews from './LatestBandNews.vue';
import AvadaQuotes from './AvadaQuotes.vue';
import LiveDates from './LiveDates.vue';

export default {
    name: "AvadaMain",
    components: { MusicIsLife, LatestBandNews, AvadaQuotes, LiveDates }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.section_width {
  width: 40%;
}

#music_is_life {
  background-color: #323844;
}
</style>