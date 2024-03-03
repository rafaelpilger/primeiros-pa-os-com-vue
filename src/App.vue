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
  <div>
  <button @click="zeradorDOcontador">zerar</button>
  <button @click="incrementarOcontador">Incrementar</button>
  <button @click="DecrementarOcontador">Decrementar</button>
  <div>
  <p>Valor do contador è : {{ contador }}</p>
</div>
  </div>
</template>

<style scoped>
  
  div{
    border-end-end-radius: 10px;
    border-end-start-radius: 10px;
    border-top-right-radius: 10px;
    border-top-left-radius: 10px;
    background-color: beige;
    padding-left: 10%;
  }
  
  button{
    font-weight: bold;
    border-radius: 111px;
    border-color: rgb(255, 0, 0);
    color: black;
    background-color: blue;
  }
  p{
    color: rgb(21, 255, 0);
    
  }
</style>
