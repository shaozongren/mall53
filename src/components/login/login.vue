<template>
    <div class="login-wrap">
        <el-form label-width="80px" :model="formdata" class="nav">
            <h2>用户登录</h2>
            <el-form-item label="用户名">
                <el-input v-model="formdata.username"></el-input>
            </el-form-item>
            <el-form-item label="密码">
                <el-input v-model="formdata.password"></el-input>
            </el-form-item>
             <el-button type="primary" class="btn" @click="handleLogin()">登陆</el-button>
        </el-form> 
    </div>
</template>
<script>
export default {
    data(){
        return{
            formdata:{
                username:"",
                password:""
            }
        }
    },
    methods:{
       async handleLogin(){ 
            //   this.$http.post('login',this.formdata).then((res)=>{
            //     console.log(res)
            const res=await this.$http.post('login',this.formdata)
                const {
                    data,
                    meta:{
                        msg,status
                    }
                }=res.data
                console.log(data,msg,status)
                if(status==200){
                    localStorage.setItem('token',data.token)
                    this.$router.push({name:'home'})
                    this.$message.success(msg)
                }else{
                    this.$message.error(msg)
                }
            // })
        }
    }
}
</script>
<style>
   .login-wrap{
       height: 100%;
       background-color: #324152;
       display:flex;
       justify-content: center;
       align-items: center;
   }
   .login-wrap .nav{
       width: 400px;
       background-color:white;
       padding:50px;
   }
   .login-wrap .nav h2{
       text-align: center;
   }
   .login-wrap .nav .btn{
       margin:0 auto;
       display: block;
   }
</style>