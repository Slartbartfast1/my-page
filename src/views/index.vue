<template>
<div>
        <header1></header1>
        <el-row :gutter="20">
            <el-col :span="18">
                <TODO></TODO>
                <questions></questions>
            </el-col>
            <el-col :span="6"><Things></Things></el-col>
        </el-row>
</div>
</template>
<script>
    import TODO from '../components/TODO.vue'
    import Things from '../components/Things.vue'
    import header1 from '../components/header1.vue'
    import questions from '../components/questions.vue'

    export default {
        name: 'index',
        components: {
            TODO, Things, header1,questions
        },
    }
</script>

<style>

</style>
