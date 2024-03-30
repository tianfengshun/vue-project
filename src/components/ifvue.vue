<template>
    <h3>条件渲染</h3>
    <div v-if = 'true'>你能看见我吗</div>
    <div v-else>你应该可以看见我吗</div>
  <div v-show = "true">你能看见我吗</div>
    <div v-if ="type === 'd'">我是ddd</div>

<!--
  v-if 渲染有较高的切换开销 当值为假是不渲染
  v-show 有较高的初始开销 少的切换开销 不论值为真假
  -->
</template>
<script>
    export default {
      data(){
        return {
          flag:true,
          type:"d"
        }
      }
    }
</script>