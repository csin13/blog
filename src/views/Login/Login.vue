<template>
  <div class="login">
    <div class="login-title">
      <h1>CSINBLOG</h1>
    </div>
    <div class="login-box">
      <div class="login-from">
        <form action="">
          <h2>LOGIN</h2>
          <p>
            <i class="iconfont icon-yonghutianchong">
              账户：
              <input
                type="text"
                v-model="from.username"
                placeholder="请输入用户名"
              />
            </i>
          </p>

          <p>
            <i class="iconfont icon-mima">
              密码：
              <input
                type="password"
                v-model="from.password"
                placeholder="请输入密码"
              />
            </i>
          </p>
          <input type="submit" value="登录" />
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      from: {
        username: "",
        password: "",
      },
    };
  },
};
</script>

<style lang="less" scoped>
.login {
  height: 100vh;
  background: url("../../assets/images/background.jpg") no-repeat;
  background-size: 100% 100%;
  color: white;
  .login-title {
    margin-left: 20px;
  }
  .login-box {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    top: 200px;
    left: 50%;
    transform: translateX(-50%);
    width: 38rem;
    height: 15rem;
    background-color: rgba(0, 0, 0, 0.6);
    border-radius: 10px;
    text-align: center;
    form {
      input {
        height: 20px;
        margin-top: 20px;
        border-bottom: 2px solid #fff;
        color: white;
        background-color: transparent;
      }
      input[type="submit"] {
        margin-top: 35px;
        width: 80%;
        height: 30px;
        font-weight: 700;
        // background-color: #f6f8fa;
        background-image: linear-gradient(to right, #74ebd5 2%, #9face6 100%);
        border-radius: 20px;
      }
    }
  }
}
</style>