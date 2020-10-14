<template>
  <div id="app">
    <h1 id="titulo">Conversor de moedas</h1>
    <div class="grupo">
      <ConversorMoedas moedaA="USD" moedaB="BRL"/>
      <ConversorMoedas moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="info">
      <h2>Free Currency Converter API</h2>
      <a href="https://free.currencyconverterapi.com">Serviço</a>
      <br>
      <br>
      <a href="https://www.currencyconverterapi.com/docs">Documentação da API</a>
    </div>
  </div>
</template>

<script>
import ConversorMoedas from './components/ConversorMoedas';

export default {
  name: 'App',
  components: {
    ConversorMoedas
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  margin: auto;
  max-width: 900px;
  background-color: rgba(242, 245, 248, 0.925);
}
#titulo {
  text-align: center;
}
.grupo {
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}
.info {
  text-align: center;
}
</style>
