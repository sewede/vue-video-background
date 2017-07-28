<template>
  <div>
    <video playsinline autoplay muted loop :poster="poster" id="bigvid">
      <source :src="videoSrcWebm" type="video/webm">
      <source :src="videoSrcMp4" type="video/mp4">
    </video>
    <div id="video-text" v-if="textOverlay">
      <h1 v-text="textHeadline"></h1>
      <h2 v-text="textSubtitle"></h2>
      <p v-text="textBody"></p>
      <a href="#" class="btn btn-primary">Contact us now</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    videoSrcWebm: {
      default: '',
      type: String
    },
    videoSrcMp4: {
      default: '',
      type: String
    },
    poster: {
      default: '',
      default: String
    }
    textOverlay: {
      default: false,
      type: Boolean
    },
    textHeadline: {
      default: '',
      type: String
    },
    textSubtitle: {
      default: '',
      type: String
    },
    textBody: {
      default: '',
      type: String
    }
  }
}
</script>

<style lang="css" scoped>
  video#bigvid {
      position: absolute;
      top: 50%;
      left: 50%;
      min-width: 100%;
      min-height: 100%;
      width: auto;
      height: auto;
      z-index: -100;
      -ms-transform: translateX(-50%) translateY(-50%);
      -moz-transform: translateX(-50%) translateY(-50%);
      -webkit-transform: translateX(-50%) translateY(-50%);
      transform: translateX(-50%) translateY(-50%);
      background-size: cover;
  }
  #video-text {
    font-weight:100;
    background: rgba(0,0,0,0.3);
    color: white;
    padding: 2rem;
    width: 33%;
    margin:2rem;
    float: right;
    font-size: 1.2rem;
    min-height: 410px;
  }
  #video-text h1 {
    color: #fff;
    font-size: 38px;
  }
  #video-text h2 {
    font-size: 28px;
    color: #fff;
  }
  #video-text p {
    font-size: 14px;
  }
</style>
