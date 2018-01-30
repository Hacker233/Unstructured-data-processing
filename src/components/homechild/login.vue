<template>
  <div>
         <el-button type="text" @click="dialogFormVisible = true" class="btn_h">SIGN   UP</el-button>

        <el-dialog title="注册" :visible.sync="dialogFormVisible">
            <el-form :model="form">
                <span class="lg_sp">用户名</span>
                <el-input v-model="input" placeholder="请输入用户名"></el-input>
                <span class="lg_sp">邮箱</span>
                <el-input v-model="input" placeholder="请输入电子邮箱"></el-input>
                <span class="lg_sp">密码</span>
                <el-input v-model="input" placeholder="请输入密码"></el-input>
                <span class="lg_sp">确认密码</span>
                <el-input v-model="input" placeholder="必须与上面密码一致"></el-input>   

            </el-form>
            <div slot="footer" class="dialog-footer">
                <el-button @click="dialogFormVisible = false">取 消</el-button>
                <el-button type="primary" @click="dialogFormVisible = false">注册</el-button>
            </div>
        </el-dialog>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        dialogTableVisible: false,
        dialogFormVisible: false,
        form: {
          name: '',
          region: '',
          date1: '',
          date2: '',
          delivery: false,
          type: [],
          resource: '',
          desc: ''
        },
        formLabelWidth: '80px'
      };
    }
  };
</script>


<style>
.btn_h{
    position: absolute;
    left: 555px;
    top: 250px;
    width: 240px;
    height: 60px;
    border-radius: 10px;
    border: none;
    background-color: rgba(138, 138, 161, 0.6);
    font-size: 20px;
    color: white;
    cursor: pointer;
    letter-spacing: 5px;
    transition:  1s;
}
.btn_h:hover{
     background-color: rgba(138, 138, 161, 1);
}
.lg_sp{
    font-size: 15px;
}
</style>

