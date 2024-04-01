<template>
      <h3>侦听器</h3>
      <p>{{message}}</p>
      <button @click = "updateHandle">修改数据 </button>
</template>


<script >
      export default {
            data(){
                  return{
                        message:"hello"
                  }
            },
            methods:{
                  updateHandle(){
                        this.message = "World"
                  }
            },
            watch:{
                  //newValue 改变后的数据
                  //oldValue 改变前的数据
                  message(newValue , oldValue){
                        console.log(newValue,oldValue)
                  }
            }
      }
</script>


<style>

</style>