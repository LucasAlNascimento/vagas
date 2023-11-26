<template>
    <div>
      <button @click="conteudo = 'home'">Home</button>
      <button @click="conteudo = 'publicar-vaga'">Publicar Vaga</button>
      <!-- renderizar de modo dinâmico os componentes home e publicar-vaga -->
      <!--<home></home>-->
      <!--<publicar-vaga></publicar-vaga>-->
      <keep-alive>
        <component :is="conteudo" />
      </keep-alive>
    </div>
  </template>
  
  <script>
  import Home from '@/components/views/Home.vue'
  import PublicarVaga from '@/components/views/PublicarVaga.vue'
  export default {
    name: 'Conteudo',
    components: {
      Home,
      PublicarVaga
    },
    data: () => ({
      conteudo: 'home'
    })
  }
  </script>
  