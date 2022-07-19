<template>
    <div class="card" v-for="(task,index) of listOfTask" :key="index" >
        <div class="card-title">
            <h3>{{task.firstName}} {{task.lastName}}</h3>
        </div>
        <div class="card-content">
            <p>{{task.comment}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        data: function(){
            return {
                listOfTask:[{
                    'firstName': 'RONAN',
                    'lastName': 'ORGO',
                    'comment' : 'The best of the best'
                }]
            }
        }
        
    }
</script>

<style>
    .card{
        width: 50%;
        border-radius: 5px;
        margin: auto;
        margin-top: 1rem;
        padding: 10px;
        box-shadow: rgba(0, 0, 0, 0.12) 0px 1px 3px, rgba(0, 0, 0, 0.24) 0px 1px 2px;
    }
</style>