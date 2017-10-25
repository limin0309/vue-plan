<!--<link rel="stylesheet" href="../../node_modules/bootstrap/dist/css/bootstrap.css">-->
<template>
  <div>
    <router-link to="/time/time-add" class="btn btn-primary">创建</router-link>
    <hr>
    <router-view></router-view>
    <hr>
    <ul class="list-group" v-for="list in lists">

      <li class="list-group-item">
        <div class="row">
          <div class="col-md-2 text-center">
            <img :src="list.avatar" class="img-circle img-responsive"><!--动态数据 用：--><!--img-circle 扁圆  img-responsive变成响应式的-->
            {{list.name}}
          </div>
          <div class="col-md-3">
            <div>
              <i class="glyphicon glyphicon-time"></i>{{list.time}}小时
            </div>
         <div class="text-info">
           <i class="glyphicon glyphicon-calendar"></i>{{list.date}}
         </div>
          </div>
          <div class="col-md-5">
            <div>
              {{list.comment}}
            </div>
          </div>
          <div class="col-md-2">
            <button class="btn-danger">&times</button><!--times 是引用的bootstrap里面的删除图标-->
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script type="text/ecmascript-6">
  import Add from '@/components/Add'
  export default{
    data(){
      return {
        lists:[
          {
            avatar: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1508907851523&di=c650b3353121477f0695271e59f58d33&imgtype=0&src=http%3A%2F%2Fimg.ishuo.cn%2Fdoc%2F1606%2F703-16061GF542.jpg',/*头像*/
            name:'jw',
            date:'2017年',
            time:'2',
            comment:'今天回去早点睡觉'
          }
        ]
      }
    },
    components: {},
    methods: {}
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
div{line-height:35px}
</style>
