<template>
  <div>
    <topo @navegar="componente = $event"></topo>
    <conteudo :conteudo="componente"></conteudo>
  </div>
</template>

<script>
import Conteudo from '@/components/layouts/Conteudo.vue'
import Topo from '@/components/layouts/Topo.vue'

export default {
  name: 'App',
  data: () => ({
    componente: 'Home'
  }),
  components: {
    Conteudo,
    Topo
  }
}
</script>

