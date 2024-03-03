<template>
  <el-divider border-style="dashed" />
  <el-space wrap>
  <el-card class="table" >
    <template #header>
      <div class="card-header">
        <span>基本信息</span>
      </div>
    </template>
    <el-table :data="tableData">
      <el-table-column prop="date" label="姓名" width="70" />
      <el-table-column prop="name" label="性别" width="60" />
      <el-table-column prop="address" label="出生日期" width="100"/>
    </el-table>
  </el-card>
  <el-card class="table">
    <template #header>
      <div class="card-header">
        <el-icon><Iphone /></el-icon>
        <span>联系方式</span>
      </div>
    </template>
    <el-table :data="tableData">
      <el-table-column prop="phone" label="手机/微信" width="120"/>
      <el-table-column prop="email" label="邮箱" width="170"/>
    </el-table>
  </el-card>
  </el-space>
  <el-divider border-style="dashed" />
</template>

<script>
import { ElCard, ElTable, ElTableColumn, ElDivider, ElSpace } from 'element-plus'
import { defineComponent } from 'vue'
export default defineComponent({
  components: {
    ElCard,
    ElTable,
    ElTableColumn,
    ElDivider,
    ElSpace
  }
})
</script>
<script setup>
const tableData = [
  {
    date: '闫锦财',
    name: '男',
    address: '1988-06-25',
    phone: '15026585943',
    email: 'yanjincai@foxmail.com'
  },

]
</script>

<style scoped>
.el-table {
  /*width: 100%;*/
  /*background-color: #ff0000;*/
  margin-top: -15px;
}
.card-header {
  padding: 0 20px;
  font-size: 18px;
  font-weight: 1000;
  color: #abaeb2;
  line-height: 5px;
  /*background-color: #0066ff;*/
}
</style>