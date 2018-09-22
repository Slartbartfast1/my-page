<template>
    <el-table
            :data="tableData"

            max-height="250">
        <el-table-column
                prop="todo"
                label="要做的事">
        </el-table-column>
        <el-table-column
                fixed="right"
                label="操作"
                width="120">
            <template slot-scope="scope">
                <el-button
                        @click.native.prevent="deleteRow(scope.$index, tableData)"
                        type="text"
                        size="small">
                    移除
                </el-button>
            </template>
        </el-table-column>
    </el-table>
</template>

<script>
    export default {
        methods: {
            deleteRow(index, rows) {
                rows.splice(index, 1);
            }
        },
        data() {
            return {
                tableData: [{todo:123},{todo:123},{todo:123},{todo:123},]
            }
        }
    }
</script>
<style scoped>

</style>