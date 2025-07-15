<template>
  <div class="componente">
    <h1>Componentes com Dados Reativos Não Primitivos</h1>
    <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>
    <button @click="fazerAniversario()">Fazer Aniversário</button>
    <button @click="mudarNome">Mudar Nome</button>
  </div>
</template>

<!-- <script setup>
import {reactive} from "vue"

  const pessoa = reactive({nome: "Igor", idade:23})

  function fazerAniversario(){
    pessoa.idade +=1
  }

  function mudarNome(){
    pessoa.nome = "Igor Ruan"
  }
</script> -->

<script>
export default{
  data:function (){
    return {
      pessoa:{
        nome:"Igor",
        idade:23
      }
    }
  },
  methods:{
    fazerAniversario:function(){
      this.pessoa.idade +=1
    },
    mudarNome:function(){
      this.pessoa.nome = "Igor Ruan"
    }
  }
}
</script>
