<template>
    <div id="app">
        <div id="logo">
            <img src="../assets/images/logo.png">
        </div>
        <h2>智慧销售管理系统</h2>
        <div id="logout" v-show="!login">
            <button @click="goto('/login')" type="button" class="mui-btn mui-btn-success">点击登录</button>
        </div>
        <div id="login" v-show="login">
            <button type="button" class="mui-btn mui-btn-success">点击进入</button>
        </div>
        <div id="copyright">
            <p>博耀信息版权所有（v1.0）</p>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                login : false //已登录状态
            }
        },
        methods: {
            goto(path) {
                this.$router.replace(path)
            }
        }
    }
</script>

<style scoped>
#app {
  background-image: url("../assets/images/login_bg.png");
  background-size : cover;
  height: 730px;
  }
#logo {
  margin: auto;
  padding-top:60px;
  width: 120px;
  height: 120px;;
}
img{
  width: 100%;
  }
h2 {
  display: block;
  text-align: center;
  margin-top: 100px;
  color: white;
}
#logout,#login{
  margin-top: 40px;
}
button{
  display: block;
  width: 120px;
  margin: auto;
}
#copyright p {
  display:block;
  text-align: center;
  margin-top: 320px;
  color: #fff;
}
</style>