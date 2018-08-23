<template>
    <div class="t_menue">
        <div class="menue_item" v-for="(item,j) in menues" :key="j">{{item}}</div>
    </div>
</template>
<style>
 .menue_item{
     font-size: 30px
 }
</style>
<script>
    module.exports = {
        name: "tmenue",
        data: function () {
            console.log(this)
            return {
                menues: ['菜单1', '菜单2', '菜单3', '菜单4']
            }
        }
    }
</script>