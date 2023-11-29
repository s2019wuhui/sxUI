<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Demo />
    <m-card 
      imgSrc="mi.jpg"
      summary="购买手机认准中国品牌，质量刚刚的,华为手机牛逼，我们必须支持！"
    />
    <br>
    <m-card 
      imgSrc="pic.jpg"
      summary="购买手机认准中国品牌，质量刚刚的,华为手机牛逼，我们必须支持！"
    >
      <template v-slot:footer>
        <div class="footer">
          <div class="level">中级 @ 345人报名</div>
          <div class="price">￥299.00</div>
        </div>
      </template>
    </m-card>
    <br>
    <m-card
      imgSrc="wb.png"
      :width="370"
      :imgHeight="90"
    >
      学习自己封装Card组件。
      <template v-slot:footer>
        <div class="footer-spring">
          <div class="level">4步骤 7门课</div>
          <div class="level">12322收藏</div>
        </div>
      </template>
    </m-card>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.footer {
  padding: 0 8px;
  font-size: 12px;
  text-align: left;
}
.level {
  color: #919991;
  margin-bottom: 8px;
}
.price {
  color: #F01414;
}
.footer-spring {
  display: flex;
  justify-content: space-between;
  padding: 0 8px;
  font-size: 12px;
}
</style>
