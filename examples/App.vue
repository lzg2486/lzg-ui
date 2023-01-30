<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Demo />
    <l-card 
    imgSrc="R-c.jpg"
    summary="测试文本123，测试文本123，测试文本123。"
    />
    <l-card 
    imgSrc="R-c (1).jpg"
    summary="测试文本123，测试文本123，测试文本123。"
    >
    <template v-slot:footer>
      <div class="footer">
        <div class="level">测试测试测试</div>
        <div class="price">$299.00</div>
      </div>
    </template>
    </l-card>
    <l-card 
    imgSrc="R-c (2).jpg"
    :width="370"
    :imgHeight="90"
    >
    测试文本456，测试文本456，测试文本456。
    <template v-slot:footer>
      <div class="footer-spring">
        <div class="level">测试测试测试</div>
        <div class="price">$299.00</div>
      </div>
    </template>
    </l-card>
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
.level{
  color: #9199A1;
  margin-bottom: 8px;
}
.price{
  color: #F01414;
}
.footer-spring{
  display: flex;
  justify-content: space-between;
  padding: 0 8px;
  font-size: 12px;
}
</style>
