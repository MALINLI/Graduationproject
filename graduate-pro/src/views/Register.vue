<template>
  <div class="register">
    <h4 class="register_tittle">注册</h4>
    <div class="register_content">
      <form action>
        <label class="ipt">
          <span class="ipt_n">姓名：</span>
          <input class="ipt_box">
        </label>
        <br>
        <label class="ipt">
          <span class="ipt_n">学校：</span>
          <input class="ipt_box">
        </label>
        <br>
        <label class="ipt">
          <span class="ipt_n">身份证号：</span>
          <input class="ipt_box">
        </label>
        <br>
        <label class="ipt">
          <span class="ipt_n">密码：</span>
          <input class="ipt_box">
        </label>
        <br>
        <label class="ipt">
          <span class="ipt_n">再次确认密码：</span>
          <input class="ipt_box">
        </label>
        <br>
        <label class="ipt">
          <span class="ipt_n">电话：</span>
          <input class="ipt_box">
        </label>
        <span style="margin-left: 10px;color:rgb(68, 128, 219); cursor: pointer;">发送验证码</span>
        <br>
        <label class="ipt">
          <span class="ipt_n">验证码：</span>
          <input class="ipt_box">
        </label>
        <br>
        <br>
      </form>
      <div class="register_btn_c">
          <router-link to="/register" style="outline:none">
            <span class="register_btn">注册</span>
          </router-link>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "register"
};
</script>
<style scoped lang="scss">
.register {
  padding: 20px;
  text-align: center;
  line-height: 260%;
  .register_content {
    text-align: left;
    width: max-content;
    margin-left: 50%;
    line-height: 260%;
    transform: translate(-50%, 0);
    .ipt {
      .ipt_n {
        display: inline-block;
        width: 100px;
        text-align: right;
      }
      .ipt_box{
        padding: 5px;
        width: 180px;
      }
    }
    .register_btn_c {
        text-align: center;
        .register_btn {
          color: #fff;
          cursor: pointer;
          border: 1px solid #eee;
          padding: 5px 40px;
          border-radius: 4px;
          background-color: rgb(68, 128, 219);
        }
      }
  }
}
</style>
