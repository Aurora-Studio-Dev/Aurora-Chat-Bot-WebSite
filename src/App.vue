<template>
  <div class="app-container">
    <header>
      <el-menu
        :default-active="activeIndex"
        class="el-menu-demo"
        mode="horizontal"
        :ellipsis="false"
        @select="handleSelect"
        background-color="transparent"
      >
        <el-menu-item index="0">
          <img
            style="width: 100px"
            src="./assets/logo.png"
            alt="Element logo"
          />
        </el-menu-item>
        <el-menu-item index="1" @click="onClickHomeNav"
          ><RouterLink to="/">首页</RouterLink></el-menu-item
        >
        <el-menu-item index="2"
          ><RouterLink to="/download">下载</RouterLink></el-menu-item
        >
        <el-menu-item index="3"
          ><RouterLink to="/about">关于</RouterLink></el-menu-item
        >
        <el-menu-item index="4"
          ><a href="https://aurorastudio.top/docs/acb">文档</a></el-menu-item
        >
        <el-sub-menu index="5">
          <template #title>友情链接</template>
          <el-menu-item index="5-1"
            ><a href="https://aurorastudio.top">Aurora Studio</a></el-menu-item
          >
          <el-menu-item index="5-2"
            ><a href="https://thzstudent.top">THZ 的博客</a></el-menu-item
          >
          <el-menu-item index="5-3"
            ><a href="https://inkore.net">iNKORE!</a></el-menu-item
          >
          <el-menu-item index="5-4">更多... </el-menu-item>
        </el-sub-menu>
      </el-menu>
    </header>
    <main>
      <RouterView />
    </main>
    <footer>
      <img src="./assets/logo.png" alt="footer" />
      <p>
        Windows 软件「 Aurora Chat Bot
        」已进行中华人民共和国计算机软件著作权登记，一切侵权行为将依法追究。
      </p>
      <p>
        计算机软件著作权登记号:
        <a href="https://www.ccopyright.com.cn/">2025SR0102045<br/>
          软著登字第14758243号</a>
      </p>
      <p>
        <a href="https://icp.gov.moe/?keyword=20240457" target="_blank">萌ICP备20240457号</a>
      </p>
      <p>Copyright © 2024 THZ(Aurora Studio). All rights reserved.</p>
    </footer>
  </div>
</template>
<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { ref } from 'vue'

const activeIndex = ref('1')
const handleSelect = (key, keyPath) => {
  console.log(key, keyPath)
}
function onClickHomeNav() {
  RouterLink.push('/')
}
</script>
<style>
.el-menu--horizontal > .el-menu-item:nth-child(1) {
  margin-right: auto;
}
a {
  text-decoration: none; /* 去除下划线 */
  color: #333; /* 字体颜色 */
}
.app-container {
  flex: 1; /* 页面其他内容填充剩余空间 */
  display: flex;
  flex-direction: column;
}
footer {
  margin-bottom: 0;
  background-color: #f3f3f3;
  padding: 10px;
  text-align: center;
}
footer img {
  width: 250px;
}
footer p {
  font-size: 16px;
  font-family: ALMM;
  color: grey;
}
</style>
