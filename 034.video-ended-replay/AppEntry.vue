<script setup lang="tsx">
import { ref, reactive, onMounted, computed } from 'vue'
const videoRef = ref<HTMLVideoElement | null>(null)

function progress(evt) {
  // console.log('progress evt: ', evt)
}
function timeupdate(evt) {
  // console.log('timeupdate evt: ', evt)
}
function ended(evt) {
  console.log('ended evt: ', evt)
  videoRef.value!.currentTime = 0
  videoRef.value!.play()
}
</script>
<template>
  <div>
    <div>不要 controls 删掉 controls 属性, 不可以是 controls="false"</div>
    <div>loop 属性存在, 不会触发 ended 事件</div>
    <div>去掉 loop 属性, ended 函数触发 currentTime=0, play, 相当于 loop</div>
    <video
      width="1000"
      autoplay
      muted
      src="/BG.mp4"
      ref="videoRef"
      @progress="progress"
      @timeupdate="timeupdate"
      @ended="ended"
    ></video>
  </div>
</template>
<style scoped lang="less">
.wrap {
  display: flex;
}
</style>
