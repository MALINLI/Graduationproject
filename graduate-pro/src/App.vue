<template>
  <div id="app">
    <div class="tittle">
      <span>教师辅助教学网站</span>
      <span class="default_head_container">
        您好，<span class="hello">xx</span>
      </span>
    </div>
    <router-view/>
    <div class="footer">
      &copy; by malinli
    </div>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  position: relative;
  height: 100%;
}
.tittle {
  height: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 28px;
  font-weight: 500;
  position: relative;
  background-color: rgb(152, 187, 219);
  .default_head_container{
    font-size: 13px;
    font-weight: 300;
    position: absolute;
    right: 20px;
    .hello{
     color: rgb(68, 128, 219);
     text-decoration: underline;
    }
  }
}
.footer{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 30px;
  color: rgb(152, 187, 219);
}
</style>
