<template>
  <h3>列表渲染</h3>
  <br/>
  <p v-for = "(item,index) in names">{{item}} - {{index}}</p>
  <div v-for=" item of result " :key = "item.id">
    <p>{{item.title}}</p>
    <P>{{item.start_datetime}}</P>
  </div>
      <div>
           <p v-for ="(value ,key ,index) of userInfo" >{{value}} - {{key}}</p>
      </div>


<!--  也可以通过v-for 处理json数据-->

</template>

<script>
  export  default {
    data(){
      return {
        names:["大宝","福福","田风顺"],
        result:[
          {
            "id": 1,
            "title": "123",
            "start_datetime": "2024-03-04 00:00:00"
          },
          {
            "id": 2,
            "title": "线下活动",
            "start_datetime": "2024-03-22 00:00:00"
          },
          {
            "id": 3,
            "title": "推送",
            "start_datetime": "2024-03-07 00:00:00"
          }
        ],
          userInfo:{
              name:"福福",
              age:10,
              sex:"女"
          }

      }
    }
  }
</script>

