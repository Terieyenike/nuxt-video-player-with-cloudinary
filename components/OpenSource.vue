<template>
  <div class="video-section">
    <p>Video.js open-source player</p>
    <video
      id="my-video"
      class="video-js vjs-big-play-centered"
      controls
      preload="auto"
      width="450"
      height="150"
      poster="https://picsum.photos/450/150"
      data-setup="{}"
    >
      <source
        src="https://res.cloudinary.com/hackit-africa/video/upload/v1639378752/nuxtjs-floating-video-player/pexels-lisa-9963201.mp4"
        type="video/mp4"
      />
      <p class="vjs-no-js">
        To view this video please enable JavaScript, and consider upgrading to a
        web browser that
        <a href="https://videojs.com/html5-video-support/" target="_blank"
          >supports HTML5 video</a
        >
      </p>
    </video>
  </div>
</template>
