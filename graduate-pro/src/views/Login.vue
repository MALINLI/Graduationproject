<template>
  <div class="login">
    <div class="login_container">
      <h4 class="login_tittle">请登录</h4>
      <form action>
        <label>
          账户：
          <input>
        </label>
        <br>
        <label>
          密码：
          <input>
        </label>
        <br>
      </form>
      <div style="margin-top: 20px;">
        <router-link to="/home" style="outline: none">
          <span class="btn">登录</span>        
        </router-link>
        <span class="line">/</span>
        <router-link to="/register" style="outline: none">
          <span class="btn">注册</span>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "login",
  props: {
    msg: String
  }
};
</script>
<style scoped lang="scss">
.login {
  padding: 35px;
  display: flex;
  justify-content: center;
  text-align: center;
  .login_container {
    padding: 35px;
    width: 380px;
    height: 180px;
    border: 1px solid #ddd;
    box-shadow: 0 0 5px #eee;
    .login_tittle {
      padding-bottom: 10px;
    }
    .btn {
      color: rgb(68, 128, 219);
      cursor: pointer;
    }
    .btn:hover{
      text-decoration: underline;
    }
    .line {
      margin: 0 6px;
    }
  }
}
</style>
