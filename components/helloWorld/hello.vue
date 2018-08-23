<template>
    <p>{{greeting}} World!</p>
</template>
<script>
    module.exports = {
        name: "hello",
        data: function () {
            return {
                greeting: "Hello"
            }
        }
    }
</script>
<style>
    p {
        font-size: 8em;
        font-weight: bold;
        text-align: center
    }
</style>