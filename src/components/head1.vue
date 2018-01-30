<template>
  <div class="nav">
    <div>
         <el-menu :default-active="activeIndex2" class="el-menu-demo nav-pad"  mode="horizontal"  @select="handleSelect"    background-color="#545c64"
  text-color="#fff"
  active-text-color="#ffd04b">
           <router-link to="/"><img src="../assets/lunbo/logo.png" alt="" class="img_l"></router-link>
           <router-link to="/"><el-menu-item index="1" class="op_1">首页</el-menu-item></router-link>
           <router-link to="/dataprocess"><el-menu-item index="/chuli"> 我的工作台</el-menu-item></router-link>
           <el-menu-item index="3">历史记录</el-menu-item>

           <el-input placeholder="请输入内容"  prefix-icon="el-icon-search"  v-model="input21" class="ipt"> </el-input>

            <div class="login">
                <el-button type="text" class="login1">登录</el-button>
                <span class="xie">/</span>
                <el-button type="text" class="login1">注册</el-button>
            </div> 
         </el-menu>
    </div>

    
  </div>
</template>

<script>
export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1',
        input:''
         
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
 body{
   margin: 0 0 0 0;
   background-color: #f5f5f5;
 }
 .login{
   float:right;
   margin-right: 30px;
   line-height: 60px;
 }
 .login1{
   color: #ffffff;
 }
 .nav-pad{
   padding-left: 50px;
  border-bottom: none;
  background-color: rgba(0, 0, 0, 0.767);
 }
.ipt{
  width: 300px;
  line-height: 60px;
  margin-left: 40px;
}
.xie{
  color: #ffffff;
}
.img_l{
  width: 40px;
  height: 40px;
  float: left;
  margin-right: 60px;
  margin-top: 12px;
}
</style>
