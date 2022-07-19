<template>
    <section>
      <friend-nav/>
      <friend-form/>
      <friend-card/>
      <friend-card/>
    </section>
</template>

<script>
import Navbar from './components/NavView.vue';
import Form from './components/FormView.vue'
import Card from './components/CardView.vue';
export default{
    components:{
      'friend-nav' :Navbar,
      'friend-form' : Form,
      'friend-card' : Card,
    }
}

</script>

<style>
  #app{
    font-family: sans-serif;
    width: 50%;
    margin: auto;
    padding: 15px;
    border-radius: 5px;
    border: 1px solid green;
  }
</style>
