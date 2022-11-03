<template>
  <main class="colums is-gapless is-multiline">
    <div class="column is-one-quarter">
      <BarraLateral />
    </div>
    <div class="column is-one-quarter">
      <FormularioAlura />
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue'
import FormularioAlura from './components/FormularioAlura.vue'

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    FormularioAlura
  }
});
</script>

<style>

</style>
