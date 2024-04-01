<template>
      <p :class="classobject">class样式绑定</p>
</template>
<script>
export default {
      data(){
            return {
                  classobject:{
                        'text-danger':true,
                         'active':true
                  }
                  }
            }

}
</script>
<style>
      .active{
            color:greenyellow;

      }
      .text-danger{
            font-size: 30px;
      }

</style>