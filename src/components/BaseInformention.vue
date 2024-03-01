<template>
  <el-table :data="tableData" style="width: 100%">
    <el-table-column prop="date" label="姓名" width="80" />
    <el-table-column prop="name" label="性别" width="60" />
    <el-table-column prop="address" label="出生日期" width="120"/>
    <el-table-column prop="phone" label="手机/微信" width="120"/>
  </el-table>
</template>

<script setup>
const tableData = [
  {
    date: '闫锦财',
    name: '男',
    address: '1988-06-25',
    phone: '15026585943'
  },

]
</script>