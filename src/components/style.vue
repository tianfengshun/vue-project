<template>
      <p :style="{color:activeColor,fontSize:fontSize+'px'}">红色</p>
</template>

<script>
      export default {
            data(){
                  return{
                        activeColor:"red",
                        fontSize:'30'
                  }
            }
      }
</script>

<style>

</style>
