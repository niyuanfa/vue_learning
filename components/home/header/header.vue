<template>
    <div class="header_box">
        <div class="header" v-for="(item,j) in headers" :key="j" @click.stop="changeItem(item,j)">
            {{item}}
        </div>
    </div>
</template>
<style>
    .header_box {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .header {
        font-size: 40px;
        padding: 10px
    }
</style>
<script>
    module.exports = {
        name: "theader",
        data: function () {
            return {
                headers: [
                    1, 2, 3, 4, 5
                ]
            }
        },
        methods: {
            changeItem(item, ind) {
                this.headers.splice(ind, 1, this.headers[ind] + 1)
            }
        }

    }
</script>