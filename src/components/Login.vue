<template>
  <div class="back">
  <el-form :rules="rules" class="login-container" label-position="left"
           label-width="0px" v-loading="loading">
    <h3 class="login_title">系统登录</h3>
    <el-form-item prop="account">
      <el-input type="text" v-model="loginForm.username" auto-complete="off" placeholder="账号"></el-input>
    </el-form-item>
    <el-form-item prop="checkPass">
      <el-input type="password" v-model="loginForm.password" auto-complete="off" placeholder="密码"></el-input>
    </el-form-item>
    <el-checkbox class="login_remember" v-model="checked" label-position="left">记住密码</el-checkbox>
    <el-form-item style="width: 100%">
      <el-button type="primary" @click.native.prevent="submitClick" style="width: 100%">登录</el-button>
    </el-form-item>
  </el-form>
</div>
</template>
<script>
  export default{
    data(){
      return {
        rules: {
          account: [{required: true, message: '请输入用户名', trigger: 'blur'}],
          checkPass: [{required: true, message: '请输入密码', trigger: 'blur'}]
        },
        checked: true,
        loginForm: {
          username: 'admin',
          password: '123'
        },
        loading: false
      }
    },
    methods: {
      submitClick: function () {
        var _this = this;
        this.loading = true;
        this.postRequest('/login', {
          username: this.loginForm.username,
          password: this.loginForm.password
        }).then(resp=> {
          _this.loading = false;
          if (resp && resp.status == 200) {
            var data = resp.data;
            console.log(data.msg);
            _this.$store.commit('login', data.msg);
            var path = _this.$route.query.redirect;
            _this.$router.replace({path: path == '/' || path == undefined ? '/home' : path});
          }
        });
      }
    }
  }
</script>
<style>
  .back{
    margin: 0px;
    padding: 0px;
    position:absolute;

    width:100%;

    height:100%;
    /* background-color: #777; */
    background-size: 100% 100%;
    background: url("https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1534156041043&di=628f4d4dad7278f5eb75102aeab14cd6&imgtype=0&src=http%3A%2F%2Fimg1.ph.126.net%2FP84GdPL7rrm0M-qUyg78Dg%3D%3D%2F58546795256266513.jpg")

  }
  .login-container {
    /* background: url("https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1534156041043&di=628f4d4dad7278f5eb75102aeab14cd6&imgtype=0&src=http%3A%2F%2Fimg1.ph.126.net%2FP84GdPL7rrm0M-qUyg78Dg%3D%3D%2F58546795256266513.jpg"); */
    border-radius: 15px;
    background-clip: padding-box;
    margin: 100px auto;
    width: 350px;
    padding: 35px 35px 15px 35px;
    background: #fff;
    border: 1px solid #eaeaea;
    box-shadow: 0 0 25px #cac6c6;
  }

  .login_title {
    margin: 0px auto 40px auto;
    text-align: center;
    color: #505458;
  }

  .login_remember {
    margin: 0px 0px 35px 0px;
    text-align: left;
  }
</style>
