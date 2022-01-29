<template>
  <video
    id="my-video"
    class="video-js"
    controls
    preload="auto"
    width="1000"
    poster="https://res.cloudinary.com/terieyenike/video/upload/vc_h264/v1643032351/video-player/mixkit-young-woman-dancing-with-a-mask-under-a-party-light.jpg"
  >
    <source src="https://res.cloudinary.com/hackit-africa/video/upload/v1639378752/nuxtjs-floating-video-player/pexels-lisa-9963201.mp4" type="video/mp4" />
    <source src="https://res.cloudinary.com/hackit-africa/video/upload/v1639378752/nuxtjs-floating-video-player/pexels-lisa-9963201.webm" type="video/webm" />
  </video>
</template>

<script>
export default {
  name: "open-source"
}
</script>

<style>
video {
  max-width: 100%;
  display: block;
}
</style>