<template>
      <div ref="conner" class="con">{{content}}</div>
      <button @click="getElementHandle">获取</button>
</template>

<script>
//无特殊需求 不要使用dom,浪费性能
export default {
      data(){
            return{
                  content:"内容",
            }
      },
      methods:{
            getElementHandle(){
                //innerHTML原生JS属性
                  console.log(this.$refs.conner.innerHTML = "哈哈哈");
            }
      }

}
</script>

<style>

</style>