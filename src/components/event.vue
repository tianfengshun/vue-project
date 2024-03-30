
<template>
      <h2>内联处理</h2>
      <button @click = "count++">数字+1</button>
      <p>当前数字是：{{count}}</p>
      <h2>方法处理器</h2>
      <button @click = "addcount">数字+1</button>
      <p>当前数字是：{{count}}</p>
</template>
<script>
export default {
      data(){
            return {
                  count:0
            }
      },
      // 所有的方法 函数 都写在这里
      methods:{
            addcount(){
                  this.count +=1;
                  this.count +=1
            }
      }
}
</script>

<style scoped>

</style>