<template>
<div>
<img class="bgimg" src="../assets/S1.jpg"/>
<h1>Hello, How are you , Welcome on my Home Page</h1> 
</div>
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
.bgimg{
    width: 1500px;
    height: 400px;
    align-items: center;
    padding-right: auto;
    box-sizing: border-box;
}
</style>