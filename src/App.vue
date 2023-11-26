<template>
  <div>
    <vagas-favoritas></vagas-favoritas>
    <topo @navegar="componente = $event"></topo>
    <alerta v-if="exibirAlerta"></alerta>
    <conteudo :conteudo="componente"></conteudo>
  </div>
</template>

<script>
import Alerta from './components/comuns/Alerta.vue';
import Conteudo from '@/components/layouts/Conteudo.vue'
import VagasFavoritas from '@/components/comuns/VagasFavoritas.vue';
import Topo from '@/components/layouts/Topo.vue'

export default {
  name: 'App',
  data: () => ({
    componente: 'Home',
    exibirAlerta: false
  }),
  components: {
    Alerta,
    Conteudo,
    VagasFavoritas,
    Topo
  },
  mounted() {
    this.emitter.on('alerta', () => {
      this.exibirAlerta = true
      setTimeout(() => 
        this.exibirAlerta = false, 4000);
    })
  }
}
</script>

