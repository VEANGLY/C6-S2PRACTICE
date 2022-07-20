<template>
    <div class="form-container">
        <form action="">
            <input type="text" placeholder="FirstName" class="form-control"><br>
            <input type="text" placeholder="LastName" class="form-control"><br>
            <input type="text" placeholder="Comment" class="form-control"><br>
            <button type="submit" class="form-control">ADD</button>
        </form>
    </div>
</template>

<script>
    export default{ 
        name: 'friemd-form',
    }
</script>
    
<style>
    .form-container{
        width: 40%;
        margin: auto;
        background: rgb(121, 174, 121);
        margin-top: 10px;
       box-shadow: rgba(0, 0, 0, 0.2) 0px 12px 28px 0px, rgba(0, 0, 0, 0.1) 0px 2px 4px 0px, rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset;
        box-sizing: border-box;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 20px;
    }
    form{
        padding:10px;
        width: 100%;
        margin: auto;
        text-align: center;
        box-sizing: border-box;
    }
   
    .form-control{
        padding: 10px;
        width: 90%;
        margin: 5px;
    }
    button{
        background: rgb(22, 237, 22);
        padding: 10px;
        margin: auto;
        font-weight: bold;
        border: none;
        color: white;
    }
</style>