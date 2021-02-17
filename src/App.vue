<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>
    <div class="linha"> 
    <Conversor moedaA="USD" moedaB="BRL"/>
     <Conversor moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="linha"> 
    <Conversor moedaA="USD" moedaB="PHP"/>
    <Conversor moedaA="PHP" moedaB="USD"/>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";

export default {
  name: 'App',
  components: {
    Conversor
  }
}
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.linha{
  margin: top;
  display: flex;
  justify-content: space-around;
}
.text-center{
  text-align: center;
}
</style>
