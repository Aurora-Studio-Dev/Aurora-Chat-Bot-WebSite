<script setup></script>

<template>
  <div id="bg" />
  <div class="hero">
    <div class="text">
      <h2>Aurora Chat Bot</h2>
      <h1>不仅仅可以聊天。</h1>
      <p>集成多款 AI 产品，使你更加方便的使用 AI 模型，提升工作效率。</p>
    </div>
    <div class="button-area">
      <el-button type="primary" size="large">下载</el-button>
      <el-button type="primary" size="large">文档</el-button>
    </div>
  </div>
  <div class="features">
    <div></div>
  </div>
</template>
<style scoped>
#bg {
  position: fixed;
  top: 0;
  left: -3%;
  width: 105vw;
  height: 105vh;
  z-index: -1;
  background: url('../assets/heroBG.png') no-repeat center center;
  background-size: cover;
}
.text h2 {
  font-size: 25px;
  font-family: MOL;
}
.text h1 {
  font-size: 45px;
  margin-top: -15px;
  font-family: ALMM;
}
.text p {
  font-size: 24px;
  font-family: OPS;
}
.hero {
  margin-top: 10%;
  margin-bottom: 15%;
  display: flex;
  flex-direction: column;
  justify-content: center; /* 垂直居中 */
  align-items: center; /* 水平居中 */
  height: 100%;
  gap: 20px; /* 调整两个区域之间的距离，增加gap */
}

.text {
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  text-align: center;
}

.button-area {
  margin: 0; /* 确保没有外边距影响布局 */
}
</style>
