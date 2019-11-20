<template>
   <div>
      <div class="wrap">
         <h2>Videos</h2>
         <Video></Video>
         <Video></Video>
         <Video></Video>
         <Video></Video>
         <Video></Video>
         <Video></Video>
         <h2>Must watch</h2>
         <VideoFullSize></VideoFullSize>
      </div>
   </div>
</template>

<script>
   import Video from '../pieces/Video';
   import VideoFullSize from '../pieces/Video-FullSize';
   export default {
      name: 'Home',
      components: { VideoFullSize, Video },
   };
</script>

<style scoped>

</style>