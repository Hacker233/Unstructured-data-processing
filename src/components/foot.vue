<template>
  <div class="footer">
    <div class="fot_u">
      <ul>
        <router-link to=""><li>团队介绍</li></router-link>
        <router-link to=""><li>联系我们</li></router-link>
        <router-link to=""><li>技术支持</li></router-link>
      </ul>
    </div>
  </div>
</template>
<script>
    
</script>
<style scoped>
.footer{
    width: 100%;
    height: 100px;
    background-color: rgb(58, 50, 50);
    margin-top: 20px;
}
li{
  float: left;
  list-style: none;
  margin-left: 200px;
  line-height: 100px;
}
.fot_u{
  margin-left: 150px;
}
.router-link-active {
    text-decoration: none;
    color: white;
    font-size: 10px;
}
.router-link-active:hover{
  color:rgb(99, 95, 91);
}
</style>

