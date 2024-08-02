<template>
    <div id="app">
        <h1>Calculadora</h1>
        <Calculator />
    </div>
</template>

<script>
import Calculator from "./main/Calculator"

export default {
    components: { Calculator }
}
</script>

<style>
@font-face {
    font-family: "RobotoMono";
    src: url("./fonts/RobotoMono-Thin.ttf");
}

* {
    font-family: "RobotoMono", monospace;
}

body {
    margin: 0;
    perspective: 1000px;
  perspective-origin: 50% 50%;
  background-color: #C7D4FB;
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;

    color: #fff;
    background: linear-gradient(to right, rgb(15, 32, 39), rgb(32, 58, 67), rgb(44, 83, 100));
}

h1 {
    transform: rotateX(20deg) rotateY(20deg);
  transform-style: preserve-3d;
  box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.2);
  color: rgb(248, 130, 27);
}
</style>