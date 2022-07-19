<template>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About us</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Help?</a></li>
        </ul>
    </nav>
</template>

<style scoped>
    nav{
        background-color: rgb(252, 47, 115);
    }
    ul{
        padding: 15px;
        display: flex;
        
    }

    li{
        list-style: none;
        margin-left: 10px;
    }
    a{
        text-decoration: none;
        color: #fff;
        text-transform: uppercase;
    }
</style>