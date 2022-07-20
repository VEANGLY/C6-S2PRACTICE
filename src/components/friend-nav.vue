<template>
    <header>
        <a href="#">Home</a>
        <a href="#"> About</a>
        <a href="#">Service</a>
        <a href="#">Help</a>
    </header>
</template>
<script>
    export default{ 
        name: 'friemd-nav',
    }
</script>
<style scoped>
   *{
       font-family: sans-serif;
   }
    header{
        padding: 20px;
        width: 100%;
        margin: auto;
        background: rgb(50, 155, 50);
    }
    header > a {
        margin: 10px;
        text-decoration: none;
        color: white;
        font-weight: bold;
    }
</style>
