<template>
    <nav>
        <div class="logo">
            <i class="el-icon-question"></i>
            <span>111</span>
        </div>
        <div class="user">
            <router-link to="/login">登陆</router-link>/
            <a href="#">注册</a>
        </div>
        <div class="search">
        <el-input  placeholder="请输入内容" suffix-icon="el-icon-search">
        </el-input>
        </div>
    </nav>
</template>
<script>
    export default {
        name: "header1"
    }
</script>

<style scoped lang="scss">
nav{
    height:60px;
    width:100%;
    background-color: darkcyan;

    .logo{
        float:left;
        height:100%;
        i{
            cursor: pointer;
            margin-left: 20px;
            font-size:50px;
            float: left;
            color: white;
            line-height:60px;
        }
        span{
            cursor: pointer;
            float: left;
            font-size:30px;
            color: white;
            line-height:60px;
            padding-left: 10px;
        }
    }
    .search{
        padding:10px 0 ;
        position: relative;
        float: right;
        width:200px;
        height: 60px;
        margin-right:10px;
    }
    .user{
        line-height:60px;
        float: right;
        margin-right:30px;
        color:white;
        a{
            text-decoration:none;
            color:white;
        }
        a:hover{
            text-decoration:underline;
        }
    }
}

</style>