<template>
  <div class="video-section player">
    <p>Native HTML Vdeo</p>
    <video
      width="450"
      height="150"
      ref="video"
      poster="https://picsum.photos/450/150"
    >
      <source :src="src" type="video/mp4" />
      Sorry, your browser doesn't support embedded videos.
    </video>
    <button title="Toggle Play" @click.prevent="togglePlay" ref="toggle">
      ►
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      src: "https://res.cloudinary.com/terieyenike/video/upload/v1643266141/video-player/gushing-waterfall.mp4",
    };
  },
  methods: {
    togglePlay() {
      const player = this.$refs.video;
      const icon = this.$refs.video.paused ? "❚ ❚" : "►";
      if (player.paused) {
        player.play();
      } else {
        player.pause();
      }
      this.$refs.toggle.textContent = icon;
    },
  },
};
</script>
