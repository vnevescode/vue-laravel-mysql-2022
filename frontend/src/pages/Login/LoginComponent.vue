<template>
    <div class="main">
        <div class="login">
            <div class="content-login">
                <header>
                    <h1>Login do sistema</h1>
                </header>
                <div class="form">
                    <form>
                        <div class="form-group">
                          <label for="exampleInputEmail1">E-mail</label>
                          <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">                          
                        </div>
                        <div class="form-group">
                          <label for="exampleInputPassword1">Password</label>
                          <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
                        </div>                        
                        <button type="submit" class="btn btn-primary login-button" @click.prevent="login">Login</button>                        
                      </form>
                </div>
            </div>
        </div>        
    </div>
</template>

<script>
export default{
    
    name: 'LoginComponent',

    data() {
        return {
            
        }
    },

    methods: {
        login(){
            this.$router.push({ name: 'Home'});
        }
    },



}
</script>

<style lang="scss" src="./style.scss" scoped />