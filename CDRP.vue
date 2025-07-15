<template>
  <div class="componente">
    <h1>Componentes com Dados Reativos Primitivos</h1>
    <p>Nome: {{ nome }} | Idade: {{ idade }}</p>
    <button v-on:click="fazerAniversario()">Fazer Aniversário</button>
    <button @click="mudarNome">Mudar Nome</button>
  </div>
</template>

<script setup>
import {ref} from "vue"

  const nome = ref("Gi")
  const idade = ref(19)

  function fazerAniversario(){
    idade.value +=1
  }

  function mudarNome(){
    nome.value = "Giovana"
  }
</script>
