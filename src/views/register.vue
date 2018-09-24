<template>
    <div>
        <div class="hero">
        </div>
        <div class="login">
            <span>注册</span>


            <router-link to="/login">
                登陆
            </router-link>
            <el-form label-position="left" label-width="80px" :model="formLabelAlign">
                <el-form-item label="用户名:">
                    <el-input></el-input>
                </el-form-item>
                <el-form-item label="密码:">
                    <el-input type="password"></el-input>
                </el-form-item>
                <el-form-item label="确认密码:">
                    <el-input type="password"></el-input>
                </el-form-item>
                <el-button type="primary">注册</el-button>
            </el-form>
        </div>
    </div>
</template>

<script>


    export default {
        name: "register",
        data() {
            return {
                labelPosition: '',
                formLabelAlign: {
                    name: '',
                    region: '',
                    type: ''
                }
            };
        }
    }
</script>

<style scoped lang="scss">

    .hero {
        background-color: #30C8CD;
        width: 100%;
        height: 350px;

    }
    span{
        position: relative;
        margin:0 auto;
        font-size:50px;
        line-height:100px;
    }

    .login {
        padding: 20px;
        position: relative;
        border-radius: 3px;
        width: 400px;
        margin: -160px auto 0 auto;
        background-color: #FFF;
        box-shadow: 0 0 10px rgba(0, 0, 0, .1);
        transition: .3s all ease;
    }

    .login:hover {
        box-shadow: 0 0 10px rgba(0, 0, 0, .3);
    }

    button {
        width: 100%;
    }
</style>