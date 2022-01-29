<template>
  <div>
    <video :src="src" autopictureinpicture ref="video"></video>
    <button title="Toggle Play" @click.prevent="togglePlay" ref="toggle">►</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      src: "https://res.cloudinary.com/terieyenike/video/upload/v1643266141/video-player/gushing-waterfall.mp4",
      isPlayed: true,
    };
  },
  methods: {
    togglePlay() {
      const player = this.$refs.video;
      const icon = this.$refs.video.paused ? '❚ ❚' : '►'
      if (player.paused) {
        player.play();
      } else {
        player.pause();
      }
      this.$refs.toggle.textContent = icon
    }
  },
};
</script>