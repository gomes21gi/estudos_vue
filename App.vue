<script setup>
import PrimeiroComponente from './PComp.vue';
import ComDados from './ComDados.vue';
import ComDadosReativosPrimitivos from './CDRP.vue';
import ComDadosReativosNaoPrimitivos from './CDRNP.vue';
</script>

<template>
  <header>Vue</header>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <ComDados/>
  <PrimeiroComponente/>
</template>
