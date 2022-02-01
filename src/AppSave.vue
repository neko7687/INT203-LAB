<script setup>
const msg = 'Hello, WORLDDDDDDDDDDD'
const counter = 0
const heading = 'color:Red'
const imagePath = '../images/images_2.jpg'
const rawHTML = '<b>BOBBY MAN</b>'
const isSearch = true
const myName = 'Preeyathorn Chaiyakum'
const score = 75
const depositAmt = 50000
// const interest = 0.1

// < 10000 = no interest
// 10000-49999 =10%
// 50000-99999 =20%
// >=100000 =25%
</script> 

<template>
    <h1>{{ msg.toLocaleLowerCase() }}</h1>
    <p>{{ counter += 10 }}</p>
    <h2 :style="heading">Ajarn Dang</h2>
    <img src="./assets/logo.png" />
    <img :src="imagePath" />
    <p v-html="rawHTML"></p>
    <div v-show="isSearch">
        <label for="search">Search</label>
        <input type="text" id="search" class="border" />
    </div>
    <p v-show="myName">Hello, {{ myName }}</p>
    <p v-if="score > 50">PASS</p>
    <p v-else-if="score == 50">EQUAL</p>
    <p v-else>HOW</p>
    <p>Deposit Amount: {{ depositAmt }}</p>
    <p v-if="depositAmt < 10000">Interest: 0</p>
    <p v-else-if="depositAmt <= 49999">Interest: {{ depositAmt * 0.1 }}</p>
    <p v-else-if="depositAmt <= 99999">Interest: {{ depositAmt * 0.2 }}</p>
    <p v-else>Interest: {{ depositAmt * 0.25 }}</p>
</template>

<style>
</style>