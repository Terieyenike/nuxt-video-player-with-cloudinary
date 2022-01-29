<template>
  <div>
    <h1>Video Players</h1>
    <cld-video publicId="video-player/grass-moving" controls width="500">
      <cld-poster publicId="image-placeholders/ht" width="500" crop="scale" quality="auto" />
    </cld-video>
    <OpenSourceVideo />
    <native-video />
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>

<style>
video, img {
  max-width: 100%;
  display: block;
}
</style>