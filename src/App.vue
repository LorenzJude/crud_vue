<script setup>
import {ref} from 'vue';
let counter = ref(0);

function add(){
  counter.value++;

}

function subtract(){
  counter.value--;

} 

</script>

<template>
  <div>
 <h1> {{ counter }} </h1>
  <button @click= "add(add)"> + </button>
  <button @click= "subtract(subtract)"> - </button>
</div>
</template>
<style>
body {
    text-align: center;
    border-style: ridge;
    border-color: blue;
    background-color: aqua;
    border-radius: 40px;
    padding-bottom: 50px;
    font-size: larger;
    font-weight: 400px;
    background: url(img/pixelblue.jpg) right bottom no-repeat, url(img/pixelblue.jpg) left top repeat;
}

h1 {    
    color: blueviolet;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

button {
    border-color: rgb(255, 0, 149);
    width: 30px;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    font-size: larger;
    color: rgb(4, 0, 253);
    font-weight: 200;
} 
</style>