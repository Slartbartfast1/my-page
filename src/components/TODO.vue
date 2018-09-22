<template>
<el-input
        type="textarea"
        :rows="2"
        placeholder="请输入内容"
        v-model="textarea">
</el-input>
</template>
<script>
    export default {
        name:'todo'
    }
</script>

<style scoped lang="scss">
 e-input{
     width:50%;
 }
</style>