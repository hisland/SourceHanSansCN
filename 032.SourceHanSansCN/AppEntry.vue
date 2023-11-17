<script setup lang="tsx">
import { ref, reactive, onMounted, computed } from 'vue'
</script>
<template>
  <div class="wrap" style="border: 1px solid #eee; padding: 10px">
    <div
      class="box"
      v-for="(vv0, index0) in [
        'SourceHanSansCN-ExtraLight',
        'SourceHanSansCN-Light',
        'SourceHanSansCN-Normal',
        'SourceHanSansCN-Regular',
        'SourceHanSansCN-Medium',
        'SourceHanSansCN-Bold',
        'SourceHanSansCN-Heavy',
      ]"
      :key="index0"
      :class="'box-' + vv0"
    >
      <div>{{ vv0 }}</div>
      <div style="font-weight: 100">abc 123 这是中文 - 100 Thin</div>
      <div style="font-weight: 200">abc 123 这是中文 - 200 ExtraLight</div>
      <div style="font-weight: 300">abc 123 这是中文 - 300 Light</div>
      <div style="font-weight: 400">abc 123 这是中文 - 400 Regular</div>
      <div style="font-weight: 500">abc 123 这是中文 - 500 Medium</div>
      <div style="font-weight: 600">abc 123 这是中文 - 600 SemiBold</div>
      <div style="font-weight: 700">abc 123 这是中文 - 700 Bold</div>
      <div style="font-weight: 800">abc 123 这是中文 - 800 ExtraBold</div>
      <div style="font-weight: 900">abc 123 这是中文 - 900 Heavy</div>
    </div>
  </div>
  <div class="wrap" style="border: 1px solid #eee; padding: 10px">
    <div>
      <div class="aa100">abc 123 这是中文 - 100 Thin</div>
      <div class="aa200">abc 123 这是中文 - 200 ExtraLight</div>
      <div class="aa300">abc 123 这是中文 - 300 Light</div>
      <div class="aa400">abc 123 这是中文 - 400 Regular</div>
      <div class="aa500">abc 123 这是中文 - 500 Medium</div>
      <div class="aa600">abc 123 这是中文 - 600 SemiBold</div>
      <div class="aa700">abc 123 这是中文 - 700 Bold</div>
      <div class="aa800">abc 123 这是中文 - 800 ExtraBold</div>
      <div class="aa900">abc 123 这是中文 - 900 Heavy</div>
    </div>
  </div>
  <div class="wrap2" style="border: 1px solid #eee; padding: 10px">
    <div>
      <div style="font-weight: 100">abc 123 这是中文 - 100 Thin</div>
      <div style="font-weight: 200">abc 123 这是中文 - 200 ExtraLight</div>
      <div style="font-weight: 300">abc 123 这是中文 - 300 Light</div>
      <div style="font-weight: 400">abc 123 这是中文 - 400 Regular</div>
      <div style="font-weight: 500">abc 123 这是中文 - 500 Medium</div>
      <div style="font-weight: 600">abc 123 这是中文 - 600 SemiBold</div>
      <div style="font-weight: 700">abc 123 这是中文 - 700 Bold</div>
      <div style="font-weight: 800">abc 123 这是中文 - 800 ExtraBold</div>
      <div style="font-weight: 900">abc 123 这是中文 - 900 Heavy</div>
    </div>
  </div>
</template>
<style scoped lang="less">
.wrap {
  display: flex;
}
.box-SourceHanSansCN-ExtraLight {
  font-family: SourceHanSansCN-ExtraLight;
}
.box-SourceHanSansCN-Light {
  font-family: SourceHanSansCN-Light;
}
.box-SourceHanSansCN-Normal {
  font-family: SourceHanSansCN-Normal;
}
.box-SourceHanSansCN-Medium {
  font-family: SourceHanSansCN-Medium;
}
.box-SourceHanSansCN-Regular {
  font-family: SourceHanSansCN-Regular;
}
.box-SourceHanSansCN-Bold {
  font-family: SourceHanSansCN-Bold;
}
.box-SourceHanSansCN-Heavy {
  font-family: SourceHanSansCN-Heavy;
}
.aa100 {
  font-family: SourceHanSansCN;
  font-weight: 100;
}
.aa200 {
  font-family: SourceHanSansCN;
  font-weight: 200;
}
.aa300 {
  font-family: SourceHanSansCN;
  font-weight: 300;
}
.aa400 {
  font-family: SourceHanSansCN;
  font-weight: 400;
}
.aa500 {
  font-family: SourceHanSansCN;
  font-weight: 500;
}
.aa600 {
  font-family: SourceHanSansCN;
  font-weight: 600;
}
.aa700 {
  font-family: SourceHanSansCN;
  font-weight: 700;
}
.aa800 {
  font-family: SourceHanSansCN;
  font-weight: 800;
}
.aa900 {
  font-family: SourceHanSansCN;
  font-weight: 900;
}
.wrap2 {
  font-family: 'Noto Sans SC';
}
</style>

<style lang="less">
@font-face {
  font-family: SourceHanSansCN-ExtraLight;
  src: url('/SourceHanSansCN-ExtraLight.otf');
}
@font-face {
  font-family: SourceHanSansCN-Light;
  src: url('/SourceHanSansCN-Light.otf');
}
@font-face {
  font-family: SourceHanSansCN-Normal;
  src: url('/SourceHanSansCN-Normal.otf');
}
@font-face {
  font-family: SourceHanSansCN-Medium;
  src: url('/SourceHanSansCN-Medium.otf');
}
@font-face {
  font-family: SourceHanSansCN-Regular;
  src: url('/SourceHanSansCN-Regular.otf');
}
@font-face {
  font-family: SourceHanSansCN-Bold;
  src: url('/SourceHanSansCN-Bold.otf');
}
@font-face {
  font-family: SourceHanSansCN-Heavy;
  src: url('/SourceHanSansCN-Heavy.otf');
}

@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-ExtraLight.otf');
  font-weight: 200;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Light.otf');
  font-weight: 300;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Normal.otf');
  font-weight: 400;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Regular.otf');
  font-weight: 500;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Medium.otf');
  font-weight: 600;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Bold.otf');
  font-weight: 700;
}
@font-face {
  font-family: SourceHanSansCN;
  src: url('/SourceHanSansCN-Heavy.otf');
  font-weight: 900;
}
</style>
