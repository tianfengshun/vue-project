<template>
      <p :style="{color:activeColor,fontSize:fontSize+'px'}">红色</p>
      <p :style="styleObject">红色22</p>
</template>

<script>
      export default {
            data(){
                  return{
                        activeColor:"red",
                        fontSize:'30',
                        styleObject:{
                              color:'green',
                              fontSize:'40px'
                        }
                  }
            }
      }
</script>

<style>

</style>
