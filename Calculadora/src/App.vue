<template>
  <div id="app">
    <h1>Calculadora Vue.js</h1>
    <Calculator />
  </div>
</template>

<script>
import Calculator from './main/calculator.vue'
export default {
    components:{Calculator}
}
</script>

<style>
@font-face {
    font-family: 'CuteFont';
    src:url('./fonts/CuteFont-Regular.ttf')
}
* {
    font-family: 'CuteFont',monospace;
}
body {
    margin:0;
}
.title {
    font-size: 40px;
}
#app {
    display:flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    background-image: linear-gradient(rgb(26, 28, 51),rgb(85, 85, 85));
}
</style>