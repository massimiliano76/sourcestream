<template>
   <div class="video full">
      <video ref="player" class="video-js">
      </video>
      <div class="bibli">
         <span class="title">There is another title to see the video</span>
         <span class="description">
            Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet,
            Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet,
            Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet,
            Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet, Lorem ipsum dolor sit amet,
         </span>
         <hr>
         <span class="viewers">Views: 10 560</span>
         <span class="tags">
            Tags:
            <span class="tag">open source</span>
            <span class="tag">open</span>
            <span class="tag">source</span>
         </span>
      </div>
   </div>
</template>

<script>
   import videojs from 'video.js';

   export default {
      name: 'Video-FullSize',

      data() {
         return ({
            player: null,
            videoOptions: {
               controls: true,
               sources: [
                  {
                     src:
                        "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ElephantsDream.mp4",
                     type: "video/mp4"
                  }
               ]
            }
         });
      },

      mounted() {
         this.player = videojs(this.$refs.player, this.videoOptions, () => {
            console.log("Player ready");
         });
      }
   };
</script>

<style scoped>

</style>