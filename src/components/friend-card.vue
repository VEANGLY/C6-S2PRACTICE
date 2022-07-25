<template>
   <div class="card">
       <h2>{{friend.FirstName}} {{friend.LastName}}</h2>
       <h5>{{friend.description}}</h5>
       <sub-friend-card v-for="(item, index) in test" :key="index" :subject="item" />
       <button class="btn">Delete</button>
   </div>
</template>

<script>
    export default{ 
        name: 'friemd-card',
        props:{
            friend:Object,
            test:Array,
        },
    }

</script>
    
<style>
   .card{
       width: 40%;
       margin:auto;
       padding: 10px;
       border-radius: 10px;
       background: rgb(242, 244, 242);
       margin-top:10px;
       box-shadow: rgba(0, 0, 0, 0.2) 0px 12px 28px 0px, rgba(0, 0, 0, 0.1) 0px 2px 4px 0px, rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset;

   }
   .btn{
       border-radius: 20px;
       padding: 10px 20px;
       margin: 5px;
   }
   h2, h5{
       font-family: sans-serif;
   }
</style>
