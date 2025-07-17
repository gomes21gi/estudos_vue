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

//const Borracha = "Borracha"
//const precoBorracha = 2.50
</script>

<template>
  <header>Vue</header>
  <RenderizacaoListas/>
  <RenderizacaoCondicional nome="Maria" :qtde-cachorros="1"/>
  <PropriedadeAssistida/>
  <PropriedadeComputada/>
  <EscutaEvento/>
  <!-- <ComProps item="Apontador" :preco="1.99"/>
  <ComProps item="Caderno" :preco="10.25"/> -->
  <!-- <ComProps :item="Borracha" :preco="precoBorracha"/> -->
  <ComProps item="Borracha" :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <ComDados/>
  <PrimeiroComponente/>
</template>