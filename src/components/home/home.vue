<template>
  <div class="home">
    <el-container class="container">
      <el-header class="header">
        <el-row class="row">
          <el-col :span="4" class="col">
            <div class="grid-content bg-purple colInner">
                
            </div>
          </el-col>
          <el-col :span="18" class="col">
            <div class="grid-content bg-purple-light colInner">
                <h3>电商后台管理系统</h3>
            </div>
          </el-col>
          <el-col :span="2" class="col">
            <div class="grid-content bg-purple colInner">
                <a href="#">退出</a>
            </div>
          </el-col>
        </el-row>
      </el-header>
      <el-container>
        <el-aside width="200px" class="aside">Aside</el-aside>
        <el-main class="main">Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>
<script>
export default {

};
</script>
<style>
.home {
  height: 100%;
}
.container {
  height: 100%;
}
.header {
  background-color: #b3c0d1;
}
.row{
    height: 100%;
}
.col{
    height: 100%;
}
.colInner{
    height: 100%;
}
h3{
    text-align: center;
}
.header img{
    height: 98%;
    width: 98%;
    display: block;
}
.aside {
  background-color: #d3dce6;
}
.main {
  background-color: #e9eef3;
}
.bg-purple{
    display: flex;
    align-items: center;
}
</style>
