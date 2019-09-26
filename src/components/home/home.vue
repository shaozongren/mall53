<template>
  <div class="home">
    <el-container class="container">
      <el-header class="header">
        <el-row class="row">
          <el-col :span="4" class="col">
            <div class="grid-content bg-purple colInner"></div>
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
        <el-aside width="200px" class="aside">
          <el-menu :unique-opened="true">
            <el-submenu index="1">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>用户管理</span>
              </template>
              <el-menu-item-group>
                 <el-menu-item index="1-1">
                     <i class="el-icon-check"></i>
                     <span>用户列表</span>
                 </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-submenu index="2">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>权限管理</span>
              </template>
              <el-menu-item-group>
                  <el-menu-item index="2-1">
                     <i class="el-icon-check"></i>
                     <span>角色列表</span>
                 </el-menu-item>
                 <el-menu-item index="2-2">
                     <i class="el-icon-check"></i>
                     <span>权限列表</span>
                 </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-submenu index="3">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>商品管理</span>
              </template>
              <el-menu-item-group>
                 <el-menu-item index="3-1">
                     <i class="el-icon-check"></i>
                     <span>商品列表</span>
                 </el-menu-item>
                 <el-menu-item index="3-2">
                     <i class="el-icon-check"></i>
                     <span>分类参数</span>
                 </el-menu-item>
                 <el-menu-item index="3-3">
                     <i class="el-icon-check"></i>
                     <span>商品分类</span>
                 </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-submenu index="4">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>订单管理</span>
              </template>
              <el-menu-item-group>
                 <el-menu-item index="4-1">
                     <i class="el-icon-check"></i>
                     <span>订单列表</span>
                 </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-submenu index="5">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>数据统计</span>
              </template>
              <el-menu-item-group>
                 <el-menu-item index="5-1">
                     <i class="el-icon-check"></i>
                     <span>数据列表</span>
                 </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
          </el-menu>
        </el-aside>
        <el-main class="main">Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>
<script>
export default {};
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
.row {
  height: 100%;
}
.col {
  height: 100%;
}
.colInner {
  height: 100%;
}
h3 {
  text-align: center;
}
.header img {
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
.bg-purple {
  display: flex;
  align-items: center;
}
</style>
