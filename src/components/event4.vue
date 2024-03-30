<template>
      <h3>数组侦听</h3>
      <button @click ="addListHandler">添加数据</button>
      <ul>
            <li v-for = "(item,index) of names " :key="index">{{item}}</li>
      </ul>

</template>


<script >
      export default {
            data(){
                  return{
                        names:["大宝","福福","田风顺"]
                  }
            },
            methods:{
                  addListHandler(){
                        //ui更新的方法
                  this.names.push("小猪");
                        //不会引起ui更新
                  //this.names.concat(["小朱"])
                  }
            }

      }

</script>


