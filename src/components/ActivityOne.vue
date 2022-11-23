<script setup>
import {ref} from "vue";


let number = ref(0);

function increment() {
    number.value ++;
}

function decrement() {
    number.value --;
}

function incrementby2() {
    number.value += 2;
}

function decrementby2() {
    number.value -= 2;
}
</script>

<template>

    <div class="textColor">{{number}}</div>
    <div class="wrapper">
    <button @click="increment()">Increment</button>
    <button @click="decrement()">Decrement</button>
    <button @click="incrementby2()">Increment by 2</button>
    <button @click="decrementby2()">Decrement by 2</button>
    </div>
</template>

<style>

.textColor{
    color: red
}

.wrapper{
    display: flex;
    grid-gap: 4%;
}
</style>