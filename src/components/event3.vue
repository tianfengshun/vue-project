<template>
      <h3>时间修饰符</h3>
      <a @click.prevent = "click1" href = "https://baidu.com">百度一下</a>
</template>


<script >
      export default {
            data(){
                  return{

                  }
            },
            methods:{
                  click1(e){
                        //阻止了a标签默认时间
                        //e.preventDefault();
                        console.log("百度");
                  }
            }
      }

</script>


