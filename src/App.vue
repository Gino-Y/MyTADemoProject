<script setup>


import Img from "@/components/Img.vue";
import Doc from "@/components/Doc.vue";
import Doc2 from "@/components/Doc2.vue";
import HelloWorld from "@/components/HelloWorld.vue";
import Show from "@/components/Show.vue";
import BaseInformention from "@/components/BaseInformention.vue";
import ZWJS from "@/components/ZWJS.vue";
</script>

<template>

  <div>
    <div class="kuang">
      <div class="h">
        <h1>个人简历</h1>
      </div>
      <div class="d">

        <div class="ii">
          <img class="i"
               src="https://mydemoshow.oss-cn-shanghai.aliyuncs.com/%E5%9B%BE%E7%89%871.jpg"
               height="128"
          >
          </img>
        </div>

        <BaseInformention/>

        <ZWJS/>

        <div class="doc">
          <h3>工作经验</h3>
          <Doc/>
        </div>

        <div class="doc2">
          <h3>教育背景</h3>
          <Doc2/>
        </div>

      </div>
    </div>
  </div>

  <div>
    <Show/>
  </div>




</template>

<style scoped>
*{
  user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  ms-user-select: none;
}
*{
  -webkit-touch-callout:none;  /*系统默认菜单被禁用*/
  -webkit-user-select:none; /*webkit浏览器*/
  -khtml-user-select:none; /*早期浏览器*/
  -moz-user-select:none;/*火狐*/
  -ms-user-select:none; /*IE10*/
  user-select:none;
}
input,textarea {
  -webkit-user-select:auto; /*webkit浏览器*/
  margin: 0px;
  padding: 0px;
  outline: none;
}
h3{
  color: white;
  margin-left: 10px;
}
.doc{
  background-color: #5d6469
}
.doc2{
  background-color: #6b7379
}
.h{
  height: 70px;
  background-color: #adb0b2;
  color: #727272;
}
.kuang{
  height: auto;
  /*background-color: #000000*/
}
.i{
  margin-top: 10px;
  margin-left: 20px;

}
.ii{
  /*background-color: red;*/
  width: 200px;
}

.d{
  width: 100%;
  height: 100%;
  /*background-color: #5d6469*/
}
h1{
  text-align:center;
  line-height:70px;
  color: #5c6369;
}
</style>
