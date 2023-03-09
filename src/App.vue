<script setup>
import HelloWorld from './components/Impuestos.vue'
import MesAñoImputacionVue from './components/Home/Archivos/Carga-de-comprobantes/Mes-año-imputacion.vue';
import ModalDeLiquidacionDelIVA from './views/liquidacionDelIVA/components/ModalDeLiquidacionDelIVA.vue';
import liquidacionDelIVA from './views/liquidacionDelIVA/liquidacionDelIVA.vue';
import LiquidacionDelIVAFecha from './views/liquidacionDelIVA/components/LiquidacionDelIVAFecha.vue';
import datosDelPeriodoFiscalAnterior from './views/personaFisica/datosDelPeriodoFiscalAnterior.vue';
import ModalDatosDelPeriodo from './views/personaFisica/ModalDatosDelPeriodo.vue';
import resImpositivoPersFisica from './views/personaFisica/resImpositivoPersFisica.vue';
</script>

<template>
  <div>
  </div>
  <resImpositivoPersFisica />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
