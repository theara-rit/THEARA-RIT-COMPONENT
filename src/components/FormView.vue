<template>
    <form action="">
        <div class="inputText">
            <input type="text" placeholder="First Name" v-model="firstName">
        </div>
        <div class="inputText">
            <input type="text" placeholder="Last Name" v-model="lastName">
        </div>
        <div class="inputText">
            <input type="text" placeholder="Comment" v-model="comment">
        </div>
        <div class="btn">
            <button @click="addInfo()">Add</button>
        </div>
    </form>

</template>

<script>
export default {
    data: function(){
        return{
            firstName: "",
            lastName: "",
            comment: "",
            listOfTask: [],
        }
    },
    methods:{
        addInfo(){
            const newInfo={
                FirstName: this.firstName,
                LastName: this.lastName,
                Comment: this.comment,
            }
            this.listOfTask.push(newInfo);
            this.firstName='';
            this.lastName = '';
            this.comment = '';
        }

    }
}
</script>

<style>
    form{
         width: 50%;
        border-radius: 5px;
        margin: auto;
        padding: 10px;
        box-shadow: rgba(0, 0, 0, 0.12) 0px 1px 3px, rgba(0, 0, 0, 0.24) 0px 1px 2px;
        margin-bottom: 10px;
    }
    .inputText{
        width: 90%;
    }
    input{
        width: 100%;
        padding: 10px;
        margin-top: 5px;
        outline: none;
    }
    button{
        width: 98%;
        padding: 10px;
        margin-top: 5px;
        color: #fff;
        background-color: #aaa;
        border: none;
        cursor: pointer;
    }
</style>