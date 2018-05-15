<template>
    <div class="page-index">
        <img src="http://oc4zuck5v.bkt.clouddn.com/yjtp.png"/>
        <input type="text" name="firstname" placeholder="电话/邮箱"/>
        <input type="text" name="firstname" placeholder="密码"/>
        <button type="button">登录</button>
    </div>
</template>

<script>
function setState(store) {}

export default {
    name: 'index',
    metaInfo: {
        title: 'Home',
        titleTemplate: '%s - Lavas',
        meta: [
            {name: 'keywords', content: 'lavas PWA'},
            {name: 'description', content: '基于 Vue 的 PWA 解决方案，帮助开发者快速搭建 PWA 应用，解决接入 PWA 的各种问题'}
        ]
    },
    async asyncData({store, route}) {
        setState(store);
    }
};
</script>

<style lang="stylus" scoped>

.page-index
    display flex
    align-items center
    flex-direction column

    input 
        
        width 80%
        height 40px
        border-style solid
        border-width  1px
        border-radius 5px
        boder-color  "#cccccc"
        padding-left 10px
        margin-top 20px

    img 
     
        margin-top 100px
        width 128px
        height 128px

    button 
       
        color #ffffff
        background #ee4000
        margin-top 20px
        width 85%
        height 40px
        border-radius 20px


</style>
