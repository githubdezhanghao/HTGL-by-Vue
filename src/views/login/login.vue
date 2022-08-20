<template>
  <div class="login">
    <h2>用户管理系统</h2>
    <el-card class="box-card">
      <el-tabs v-model="activeName" @tab-click="handleClick" :stretch="true">
        <el-tab-pane label="密码登录" name="first">密码登录</el-tab-pane>
        <el-tab-pane label="短信登录" name="second">短信登录</el-tab-pane>
      </el-tabs>
    </el-card>
  </div>
</template>

<script>
import '../../assets/css/login.scss'
export default {
  data() {
    return {
      activeName: "second",
    };
  },
  methods: {
    handleClick(tab, event) {
      //   console.log(tab, event);
    },
  },
};
</script>

<style lang="scss" scoped>

</style>
