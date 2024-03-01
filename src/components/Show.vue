<template>
  <el-card class="box-card">
<!--    <el-image>123</el-image>-->
<!--      <img-->
<!--          src="../assets/故障效果-1.gif"-->
<!--          alt="展示的图片"-->
<!--          width=100%-->
<!--          height=100%-->
<!--          object-fit:cover;-->
<!--      >-->
    <Plane/>
  </el-card>
</template>
<style scoped>
.text {
  font-size: 14px;
}

.item {
  padding: 18px 0;
}

.box-card {
  width: 100%;
  height: 100%;
  background-color: #5c6369;
}
</style>
<script>
import Plane from "@/components/Plane.vue";
export default {
  components: {Plane}
}
</script>