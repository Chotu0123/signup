<template>
<img class="logo" src="../assets/S1.jpg"/>
<h1>Hello, How are you , Welcome on my Home Page</h1> 
</template>
<script>
export default{
    name: "Home",   
    mounted()
    {
      let user= localStorage.getItem('user-info');
      if(!user)
      {
        this.$router.push({name:'SignUp'})
      }
    }
}
</script>

<style>
.logo{
    width: 400px;
}
</style>