<template>
  <div class="head-portrait">
    <!-- <img :src="imgUrl" alt=""> -->
    <!-- <div class="head-avatar"></div> -->

  <div class="status" id="status"></div>

  </div>
  <!-- <div class="head-portrait"> -->
    <!-- <img :src="imgUrl" alt=""> -->
    <!-- <div class="head-avatar"></div> -->

  <!-- <div class="status" id="status"></div> -->
  <!-- <div class="status" style="z-index: index 999999999; background-color:red;" id="status2"></div> -->

  <!-- </div> -->
</template>

<script>
import {USER_HEAD_IMG_URL} from '@/store/mutation-types'
export default {
    props: {
        imgUrl:{ default:USER_HEAD_IMG_URL}
    }
}
</script>

<style lang="scss" scoped>
.head-portrait {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color:#7BA698;
    // border: 2px solid rgb(137,140,151);
    // border: 2px solid rgb(255, 255, 255);
    position: relative;
    .status {
        content: '';
        width: 12px;
        height: 12px;
        z-index: 1;
        display: block;
        border-radius: 50%;
        background-color: #42FF00;
        position: absolute;
        right: 0;
        bottom: 0;
    }
    .head-avatar {
        width: 45px;
        height: 45px;
        border-radius: 50%;
        // padding: 2px;
        box-sizing: border-box;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        vertical-align: middle;
    }
}
</style>