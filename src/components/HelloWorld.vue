<template>
  <div class="hello">
     
　　 <!-- 外层盒子 -->
    <div style="height:200px;width:600px;background-color:#fff; margin:0px auto;">
      <!-- 这里的标签名称要和main.js文件中定义的组件名称保持一致 -->
      <happy-scroll color="rgba(0,0,0,0.5)" size="0" resize hide-horizontal>
        <!-- 内层盒子——内容区 -->
        <div class="con">
          <ol>
            <li><span class="text6">&nbsp;&nbsp;支持上传 xls 和 xlsx 格式的数据.</span></li>
            <li><span class="text6">&nbsp;&nbsp;EXCEL文件名任意，表格名“Sheet1”.</span></li>
            <li><span class="text6">&nbsp;&nbsp;字段依次为“厂家”，“表型”，“时间”，“值”</span></li>
            <li><span class="text6">“厂家”和“表型”的组合必须在《水表型号数据》的表格中有记录对应.</span></li>
            <li><span class="text6">“时间”格式任意.</span></li>
            <li><span class="text6">“值”格式文本和数值都可以，也可以为空，数据为单位小时的水量数据（ m³/h ），可以是类似流量计的瞬时流
          量，也可以是类似水表的每小时的累积水量，自来水公司会有类似日报的小时水量统计数据表，这些都是符合要求
          的数据。但程序能成功选型的条件是至少有100条有效的数据，当然数据越多越好。</span></li>
            
          </ol>
        </div>
      </happy-scroll>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.con {
  width: 490px;
  text-align: start;
  line-height:30px;
  text-indent:0em
}

ol{
  list-style: num;
  color:#e2e5e8;
  height: 300px;
}
ol>li{
  height: 30px;
  width: 490px;
 /*  border-bottom:1px #6e7b8b solid; */
}
.text6{
 font-family: "微软雅黑";
  font-size: 14px;
  
  color: #6e7b8b;
}
</style>
