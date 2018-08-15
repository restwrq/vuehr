<template lang="html">
  <div class="back1"
  <div class="inback1">
    <h1>履历</h1>
    <el-row>
  <el-col :span="24"><div class="grid-content bg-purple-dark"></div></el-col>
</el-row>
<el-row>
  <el-col :span="12"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="12"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
<el-row>
  <el-col :span="8"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="8"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="8"><div class="grid-content bg-purple"></div></el-col>
</el-row>
<el-row>
  <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="6"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="6"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
<el-row>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
<el-row>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
<el-row>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="4"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
<el-row>
  <el-col :span="12"><div class="grid-content bg-purple"></div></el-col>
  <el-col :span="12"><div class="grid-content bg-purple-light"></div></el-col>
</el-row>
</div>
</div>
</template>

<script>
export default {
  data() {
     return {
       tableData3: [{
         date: '2016-05-03',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-02',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-04',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-01',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-08',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-06',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }, {
         date: '2016-05-07',
         name: '王小虎',
         province: '上海',
         city: '普陀区',
         address: '上海市普陀区金沙江路 1518 弄',
         zip: 200333
       }]
     }
   }
}
</script>

<style lang="css">
.inback1{
  position: relative;
  /* width: 30%; */
  right: -25%;
  width: 50%;
  text-align: center;
}

.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>
