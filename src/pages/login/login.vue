<template>
    <div>
        <button @click="getData" class="mui-btn mui-btn-primary">获取数据</button>
    </div>
</template>

<script>
export default {

  methods: {
    getData() {
      let url = "http://218.23.119.102:9088/train-rest/rest/user/login"
      let user = {}
      user.loginName = "2016238"
      user.password = "123456"
      let userjson = JSON.stringify(user)
      this.$http.post(url, userjson,{emulateJSON : true} )
        .then(
          response => {
            console.log(response)
          },
          response => {
            console.log(
              "发送失败" + response.status + "," + response.statusText
            )
          }
        )
       
    }
  }
}
</script>

<style scoped>
</style>