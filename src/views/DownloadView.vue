<template>
  <h1>下载中心</h1>
  <div class="Most">
    <h4>下载最新版本</h4>
    <h2>Release v1.0.1</h2>
    <el-divider/>
    <h3>更新日志</h3>
    <p>
      [Fix] 长文本显示不全
      <br/>
      [Change] HomePage & ChatPage 布局修改
      <br/>
      [Change] SettingPage Border --> SettingsCard & Expander --> SettingsExpander
      <br/>
      [Change] 主页金句 API 修改
      <br/>
      [Delete] 天气预留位
      <br/>
      [Add] ToolsPage
      <br/>
      [Add] Markdown 格式显示渲染支持
    </p>
    <el-divider/>
    <el-button onclick="window.open('https://github.com/Aurora-Studio-Dev/Aurora-Chat-Bot/releases/tag/Releases')" color="black" size="large" round>Github</el-button>
    <el-button onclick="window.open('https://www.123865.com/s/9GLUVv-jfQwh')" type="primary" size="large" round>123云盘</el-button>
    <el-button onclick="window.open('https://thzstudent.lanzouu.com/i514D2okxhah')" color="orange" size="large" round>蓝奏云 （密码：fvwq）</el-button>
  </div>
</template>
<script setup>
</script>
<style scoped>
h1 {
  font-family: ALMM;
  font-size: 35px;
  text-align: center;
  margin-top: 35px;
}
.Most {
  margin-left:10%;
  margin-top: 35px;
  margin-right: 10%;
  margin-bottom: 45px;
}
p{
  font-family: OPS;
}
h3 ,h2{
  font-family: ALMM;
}
</style>
