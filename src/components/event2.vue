<template>
      <h2>事件传参</h2>
      <p>也可以传递event对象</p>
      <p @click= "getNameHandler(item,$event)" v-for ="(item , index ) of names" :key = "index">{{item}}</p>
</template>
<script>
export default {
      data(){
            return {
                  names:["大宝","福福","田风顺"]
            }
      },
      // 所有的方法 函数 都写在这里
      methods:{
           getNameHandler(name,e){
                 console.log(name);
                 console.log(e);
           }
      }
}
</script>