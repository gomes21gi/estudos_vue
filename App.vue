<script setup>
import PrimeiroComponente from './PComp.vue';
import ComDados from './ComDados.vue';
import ComDadosReativosPrimitivos from './CDRP.vue';
import ComDadosReativosNaoPrimitivos from './CDRNP.vue';
import DataBinding from './DB.vue'
import ComProps from './ComProps.vue'
import EscutaEvento from './EsE.vue'
import PropriedadeComputada from './ProComp.vue'
import PropriedadeAssistida from './ProAss.vue'
import RenderizacaoCondicional from './RC.vue'
import RenderizacaoListas from './RL.vue'
import Slots from './Slots.vue'

const Borracha = "Borracha"
const precoBorracha = 2.50

const cachorrosDoJoao = [
  {nome:"Totó", idade:2},
  {nome:"Tico", idade:8},
  {nome:"Teco", idade:11}
]
</script>

<template>
  <header>Vue</header>
  <Slots>
    <template v-slot:icone>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512"><!--!Font Awesome Free 6.7.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2025 Fonticons, Inc.--><path fill="#ffffff" d="M575.8 255.5c0 18-15 32.1-32 32.1l-32 0 .7 160.2c0 2.7-.2 5.4-.5 8.1l0 16.2c0 22.1-17.9 40-40 40l-16 0c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1L416 512l-24 0c-22.1 0-40-17.9-40-40l0-24 0-64c0-17.7-14.3-32-32-32l-64 0c-17.7 0-32 14.3-32 32l0 64 0 24c0 22.1-17.9 40-40 40l-24 0-31.9 0c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2l-16 0c-22.1 0-40-17.9-40-40l0-112c0-.9 0-1.9 .1-2.8l0-69.7-32 0c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z"/></svg>
    </template>
    <template v-slot:texto>
      Home
    </template>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512"><!--!Font Awesome Free 6.7.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2025 Fonticons, Inc.--><path fill="#ffffff" d="M575.8 255.5c0 18-15 32.1-32 32.1l-32 0 .7 160.2c0 2.7-.2 5.4-.5 8.1l0 16.2c0 22.1-17.9 40-40 40l-16 0c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1L416 512l-24 0c-22.1 0-40-17.9-40-40l0-24 0-64c0-17.7-14.3-32-32-32l-64 0c-17.7 0-32 14.3-32 32l0 64 0 24c0 22.1-17.9 40-40 40l-24 0-31.9 0c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2l-16 0c-22.1 0-40-17.9-40-40l0-112c0-.9 0-1.9 .1-2.8l0-69.7-32 0c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z"/></svg>
    Home
  </Slots>
  <RenderizacaoListas nome="João" :cachorros="[]"/>
  <RenderizacaoListas nome="João" :cachorros="cachorrosDoJoao"/>
  <RenderizacaoCondicional nome="Maria" :qtde-cachorros="1"/>
  <PropriedadeAssistida/>
  <PropriedadeComputada/>
  <EscutaEvento/>
  <ComProps item="Apontador" :preco="1.99"/>
  <ComProps item="Caderno" :preco="10.25"/>
  <ComProps :item="Borracha" :preco="precoBorracha"/>
  <ComProps item="Borracha" :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <ComDados/>
  <PrimeiroComponente/>
</template>
