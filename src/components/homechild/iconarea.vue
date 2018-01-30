<template>
<div class="icontubiao">
  <div class="divimg">
    <router-link to="../dataprocess" class="link_a">
      <img src="../../assets/lunbo/jieguo.png" alt="">
      <p>数据处理</p>
    </router-link>
  </div>
  <div class="divimg">
    <router-link to="" class="link_a">
      <img src="../../assets/lunbo/chuli.png" alt="">
      <p>结果展示</p>
    </router-link>
  </div>
  <div class="divimg">
    <router-link to="" class="link_a">
      <img src="../../assets/lunbo/yangli.png" alt="">
      <p>案例分析</p>
    </router-link>
  </div>
</div>
</template>
<style scoped>
.icontubiao{
  height: 300px;
  text-align: center;
  padding-left: 160px;
  border: none;
  margin-bottom: 30px;
}
.divimg{
  width: 200px;
  height: 100px;
  float: left;
  margin-right: 20px;
  text-align: center;
  line-height: 300px;
  margin-left: 100px;
    transition: 1s;
}
img{
  margin-right: 30px;
  width: 100px;
  height: 100px;
  color: #333;

}
.divimg:hover{
    transform: scale(1.2);
}
p{
  margin-top: -260px;
  margin-left: -35px;
  font-size: 18px;
  color: #666;
}
.link_a{
  text-decoration: none;
}
</style>

