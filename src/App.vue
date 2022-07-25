<template>
    <friend-nav/>
    <friend-form @add-data="addFriend"/>
    <friend-card v-for="friend of friends" :key="friend" :friend="friend" :test="subCard" />
</template>


<script>
    export default{
        name:'App',
        data(){
            return {
                friends:[],
                subCard:[],
                object:{FirstName:null,LastName:null,description:null,}
                
            }
        },
        methods:{
            addFriend(fname, lname, comment,newSkill){
                this.friends.push({FirstName:fname, LastName: lname,description:comment});
               this.subCard = newSkill
               console.log(comment);
            }

        }
    }
</script>