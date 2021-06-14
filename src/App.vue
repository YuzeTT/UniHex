<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style>
body{
  padding: 0;
  margin: 0;
  background-color: #252A44;
}

/* 提权-menu下拉菜单样式 */
.el-menu--horizontal>.el-submenu .el-submenu__title {
  height: 48px;
  line-height: 48px;
  color: hsla(0,0%,100%,.8);
}

/* 提权-menu下拉菜单选中颜色 */
.el-menu--horizontal>.el-submenu.is-active .el-submenu__title {
  color: #FFFFFF;
}

/* 提权-menu下拉菜单hover颜色 */
.el-menu--horizontal>.el-submenu:focus .el-submenu__title, .el-menu--horizontal>.el-submenu:hover .el-submenu__title {
  color: #FFFFFF;
}

/* 提权-menu下拉菜单底部描边 */
.el-menu--horizontal>.el-submenu.is-active .el-submenu__title {
  border-bottom: 3px solid #2483ff;
}

/* 提权-menu菜单下拉按钮背景色 */
.el-menu--horizontal> .el-menu-item:not(.is-disabled):focus, .el-menu--horizontal>.el-menu-item:not(.is-disabled):hover, .el-menu--horizontal>.el-submenu .el-submenu__title:hover {
  background-color: #131625;
}

/* 提权-menu下拉菜单宽度 */
.el-menu--collapse .el-menu .el-submenu, .el-menu--popup {
    min-width: 102px;
}

/* 提权-menu下拉菜单描边缩小 */
.el-submenu__title {
  padding: 0;
  margin: 0 10px;
}

/* 提权-menu菜单背景色 */
.el-menu{
  background-color: #131625;
}

/* 提权-menu下拉菜单背景色 */
.el-menu--horizontal .el-menu .el-menu-item, .el-menu--horizontal .el-menu .el-submenu__title {
  background-color: #131625;
}
</style>
