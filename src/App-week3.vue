<script setup>
function printMessage() {
    console.log('Hello, function')
}
//call/execute function
printMessage()
//2. function expression
const showMessage = function (msg) {
    console.log(`Hello,${msg}`)
}

showMessage('this is a function expression')

</script>
 
<template></template>
 
<style>
</style>