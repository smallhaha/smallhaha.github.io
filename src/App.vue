<!--
 * @Author: your name
 * @Date: 2021-12-21 15:16:35
 * @LastEditTime: 2022-03-21 16:34:02
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vuedeomo3\src\App.vue
-->
<template>
  <router-view />
</template>
<script>
export default {
  name: "App",
  mounted() {
    /**
     * 解决 css 引入图片在 github pages 无法获取的问题
     */
    const { NODE_ENV } = process.env;
    document.documentElement.className = NODE_ENV;
  }
};
</script>
<style lang="less">
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  font-family: "PingFangSC-Regular", "Microsoft YaHei";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #666;
}
* {
  margin: 0;
  padding: 0;
}
.main_display {
  display: flex;
  justify-content: end;
  align-items: center;
}
</style>
