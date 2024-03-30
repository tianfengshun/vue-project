<template>
    <h3>{{home.name}}</h3>
    <p>{{ tfsContent }}</p>
    <p>{{ tfsContent1() }}</p>
</template>


<script >
    export default {
        data(){
                return{
                    home:
                    {
                        name:"小田家",
                        play:["大宝","福福","田风顺"]
                }
            }
        },
        //计算属性与方法都可实现以下内容，计算后的值代码未更改保存在缓存中，可以多次调用，无需重新计算
        //而方法属性，每次调用都会重新渲染
        computed:{
            tfsContent(){
                return this.home.play.length>0 ? '有人' : '没人';
            }
        },
        methods:{
            tfsContent1(){
                return this.home.play.length>0 ? '有人' : '没人';
            }
        }

    }

</script>

