<script setup>
import { ref } from 'vue'

// El contador empieza en cero
const count = ref(0)

// Funciones para el plan de pruebas
const aumentar = () => {
  if (count.value < 10) count.value++
}

const disminuir = () => {
  if (count.value > 0) count.value--
}

</script>

<template>
  <div style="text-align: center; padding: 20px;">
    <h1>Contador DAW</h1>
    <h2>{{ count }}</h2>
    
    <button @click="aumentar">Incrementar (+)</button>
    <button @click="disminuir" style="margin-left: 10px;">Decrementar (-)</button>
    
    <p v-if="count === 10" style="color: red;">Límite máximo alcanzado (10)</p>
    <p v-if="count === 0" style="color: blue;">Límite mínimo alcanzado (0)</p>
  </div>
</template>
