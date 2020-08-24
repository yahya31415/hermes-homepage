<template>
  <div id="cover-video">
    <video src="@/assets/cover.mp4" autoplay preload="auto" loop muted></video>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss">
#cover-video {
  position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
  video {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 100% 100%;
  }
}
</style>
