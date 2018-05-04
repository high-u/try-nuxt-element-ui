<template>  
  <div>
    <el-header>
      <nav-bar />
    </el-header>
    <el-container>
      <el-aside width="auto">
        <side-bar />
      </el-aside>
      <el-main>
        <nuxt class="centered-text"/>
      </el-main>      
    </el-container>
    <el-footer>
      <my-footer/>
    </el-footer>
  </div>
</template>

<script>
import MyFooter from '~/components/Footer.vue'
import NavBar from '~/components/NavBar.vue'
import SideBar from '~/components/SideBar.vue'

export default {
  components: {
    MyFooter,
    NavBar,
    SideBar
  }
}
</script>

<style>
html, body {
  padding: 0;
  margin: 0;
  height: 100%;
  width: 100%;
}
.el-header {
  background-color: #545c64;
  line-height: 60px;
}
.el-aside {
  border-right: 1px solid #E4E7ED;
}
.el-footer {
  border-top: 1px solid #E4E7ED;
}
.centered-text {
  text-align: center;
}
</style>
