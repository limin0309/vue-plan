<!--<link rel="stylesheet" href="../../node_modules/bootstrap/dist/css/bootstrap.css">-->
<template>
  <div>
    <div class="navbar navbar-default">
      <!--nav-default 灰色-->
      <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand">计划表
            <i class="glyphicon glyphicon-time"></i>
          </a>
        </div>
        <ul class="navbar-nav nav">
          <li>
            <router-link to="/home">首页</router-link>
          </li>
          <li>
            <router-link to="/time">计划列表</router-link>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default{
    data(){
      return {}
    },
    components: {},
    methods: {}
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">

</style>
