<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <el-container>
      <el-header style="height:48px;padding: 0px;background-color: #131625;">
        <p style="float: left;line-height: 10px;">qwq</p>
        <!-- header -->
        <el-menu style="height:48px;float: left;" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
          <!-- header-left -->
          
          <el-menu-item index="1">主页</el-menu-item>
          <!-- <el-menu-item index="2">主页</el-menu-item> -->
          <!-- <el-submenu index="3">
            <template slot="title">工作台</template>
            <el-menu-item index="3-1">选项1</el-menu-item>
            <el-menu-item index="3-2">选项2</el-menu-item>
            <el-menu-item index="3-3">选项3</el-menu-item>
          </el-submenu> -->
          <el-submenu index="2" style="height: 48px;line-height: 48px">
            <template slot="title" style="height: 48px;line-height: 48px">工作台</template>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item>
          </el-submenu>
          <!-- header-right -->
          
        </el-menu>
        <div class="uniui-header-right">
            <el-button type="primary" size="small">主要按钮</el-button>
        </div>
        <!-- header end -->
      </el-header>
      <el-main>Main</el-main>
      <el-footer>Footer</el-footer>
    </el-container>
    
    
    <!-- body -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
  },
  data() {
    return {
      activeIndex: '1',
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>

<style scoped>
.uniui-header-left {
  float: left;
}

/* ui顶部右对齐 */
.uniui-header-right {
  float: right;
  line-height: 48px;
  padding: 0 10px;
}

/* menu选项样式 */
.el-menu--horizontal>.el-menu-item {
  height:48px;
  line-height: 48px;
  color: hsla(0,0%,100%,.8);
  padding: 0 2px;
  margin: 0 20px;
}

/* menu底部描边 */
.el-menu {
  border-bottom: none;
  
}

/* menu激活颜色和描边 */
.el-menu-item.is-active {
  color: #FFFFFF;
  border-bottom: 3px solid #2483ff;
}

/* menu选中后颜色 */
.el-menu--horizontal > .el-menu-item:not(.is-disabled):focus, .el-menu-item:not(.is-disabled):hover {
    color: #FFFFFF;
}

.el-menu--horizontal>.el-submenu .el-submenu__title {
  height: 48px;
  line-height: 48px;
}

/* menu下拉激活颜色和描边 */
.el-menu--popup-bottom-start >.el-menu-item.is-active {
  color: #FFFFFF;
  border-bottom: none;
  background-color: #131625;
}

.el-menu {
  background-color: #131625;
}

/* .el-menu--popup-bottom-start > .el-menu-item:not(.is-disabled):focus, .el-menu-item:not(.is-disabled):hover{
  color: #2483ff;
} */
.el-menu--popup-bottom-start > .el-menu{
  background-color: #2483ff;
}
/* 
.el-menu--popup-bottom-start >.el-menu-item.is-active {
  color: #2483ff;
  background-color: rgba(242,246,250,.7);
} */


</style>