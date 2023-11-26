<template>
  <div>
    <vagas-favoritas></vagas-favoritas>
    <topo @navegar="componente = $event"></topo>
    <conteudo :conteudo="componente"></conteudo>
  </div>
</template>

<script>
import Conteudo from '@/components/layouts/Conteudo.vue'
import VagasFavoritas from '@/components/comuns/VagasFavoritas.vue';
import Topo from '@/components/layouts/Topo.vue'

export default {
  name: 'App',
  data: () => ({
    componente: 'Home'
  }),
  components: {
    Conteudo,
    VagasFavoritas,
    Topo
  }
}
</script>

