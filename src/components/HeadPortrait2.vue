<template>
  <div class="profile">
    <div class="name" style="height: 50px; line-height: 50px">GPT-Fail</div>
    <div class="status" id="avatar-status"></div>
  </div>
</template>

<script>
import { USER_HEAD_IMG_URL } from "@/store/mutation-types";
export default {
  props: {
    imgUrl: { default: USER_HEAD_IMG_URL },
  },
};
</script>

<style lang="scss" scoped>

.profile {
  display: flex;
  flex-direction: row;
  align-items: baseline;
  gap: 8px;
  background-color: dodgerblue;
  padding: 0 20px;

  .name {
font-family: 'TestSöhne';
    font-size: 20px;
    color: #ffffff;
    // letter-spacing: 110%;
  }
}
.status {
  content: "";
  width: 15px;
  height: 15px;
  z-index: 1;
  display: block;
  border-radius: 50%;
  background-color: #42ff00;
}
</style>