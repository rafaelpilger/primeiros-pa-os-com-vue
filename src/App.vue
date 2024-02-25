<script setup>
import { ref } from 'vue';

const contador = ref(0);

function incrementarOcontador() {
  contador.value++;
}

function DecrementarOcontador() {
  if (contador.value > 0){
     contador.value--;
  }
}

function zeradorDOcontador() {
  contador.value = 0;
}

</script>

<template>
  <div class="botoes">
  <button @click="zeradorDOcontador">zerar</button>
  <button @click="incrementarOcontador">Incrementar</button>
  </div>
  <button @click="DecrementarOcontador">Decrementar</button>
  <div class="zerador">
  <p>Valor do contador è : {{ contador }}</p>
  </div>
</template>

<style scoped>
  button{
    font-weight: bold;
    border-radius: 30px;
    border-color: aqua;
    color: blue;
  }
  p{
    color: red;
  }
</style>
