<template>
  <transition name="guodu">
      <div class="cont">
      <div class="head1">
          <p class="dataclo">非结构化数据转化为结构化数据</p>
      </div>
      <div>
        <el-input class="areatxt"  type="textarea"  :rows="10"  placeholder="请复制或者上传待处理的数据内容"  v-model="textarea"></el-input>

      </div>
      <div class="btncon">
         <div class="btncon-1">
                <el-button type="primary">上传<i class="el-icon-upload el-icon--right"></i></el-button>&nbsp;&nbsp;&nbsp;&nbsp;
                <el-button-group>
                <el-button type="primary">开始分析</el-button>
                <el-button type="primary">来个demo</el-button>
                <el-button type="primary">清空</el-button>
                </el-button-group>

                <el-select v-model="value" placeholder="请选择展现方式">
                    <el-option  v-for="item in options"  :key="item.value"  :label="item.label"  :value="item.value"></el-option>
                </el-select>
         </div>
      </div>
      <div>
           <el-input class="areatxt"  type="textarea"  :rows="10"  placeholder="分析结果"  v-model="textarea"></el-input>
      </div>
  </div>
  </transition>
</template>


<script>
export default {
  data() {
    return {
            textarea: '',
             fileList3: [{
                             name: 'food.jpeg',
                             url: 'https://fuss10.elemecdn.com/3/63/4e7f3a15429bfda99bce42a18cdd1jpeg.jpeg?imageMogr2/thumbnail/360x360/format/webp/quality/100',
                              status: 'finished'
                         }, {
                            name: 'food2.jpeg',
                            url: 'https://fuss10.elemecdn.com/3/63/4e7f3a15429bfda99bce42a18cdd1jpeg.jpeg?imageMogr2/thumbnail/360x360/format/webp/quality/100',
                            status: 'finished'
                         }],
             options: [{
                        value: '选项1',
                        label: '文本方式展现'
                        }, {
                        value: '选项2',
                        label: '柱状图'
                        }, {
                        value: '选项3',
                        label: '饼状图'
                        }, {
                        value: '选项4',
                        label: '折线图'
                        }, {
                        value: '选项5',
                        label: '树状图'
                        }],
                        value: ''
                  };
              },
    methods: {
      handleChange(file, fileList) {
        this.fileList3 = fileList.slice(-3);
      }
    },
  
}
</script>
<style scoped>
.cont{
    height: 650px;
    width: 1180px;
    box-sizing: border-box;
    margin: 0 auto;
   border: none;
    margin-top: 30px;
    text-align: center;
    border: 1px solid rgb(168, 154, 154);
}
.head1{
    height: 60px;
    width: 100%;
    background-color:#43a6f1;
    border:none;
    margin-bottom: 20px;
    line-height: 60px;
    box-sizing: border-box;
    margin-top: -16px;
}
.areatxt{
    width: 1130px;
    margin-bottom: 10px;
    background-color: rgb(231, 210, 210);
    border:none;
}
.btncon{
    width: 1130px;
    height: 50px;
    margin: 0 auto;
    margin-bottom: 10px;
    line-height: 50px;
    border:none;
}
.btncon-1{
    float: left;
    margin-left: 5px;
    margin-right: 10px;
    border:none;
}
.dataclo{
    color: #ffffff;
}
.guodu-enter, .guodu-fade-leave-active { 
  opacity: 0; 
} 
.guodu-enter-active, .guodu-leave-active {
   transition: opacity 1s ease 
}
</style>
