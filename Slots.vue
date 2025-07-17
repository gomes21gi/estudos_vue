<script setup></script>

<template>
  <div class="componente">
    <h1>Componentes com Slots</h1>
    <button>Botão</button>
    <button><slot></slot></button>
    <button><slot name="icone"/> <slot name="texto"/></button>
    <button>
      <slot name="icone"/>
      <slot name="texto"/>
      Botão
    </button>
  </div>
</template>
