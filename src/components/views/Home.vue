<template>
    <div class="container py-4">
        <div class="row">
            <div class="col">  
                <pesquisar-vaga></pesquisar-vaga>
            </div>
        </div>
        
        <div class="row mt-5">
            <div class="col-4">
                <indicador titulo="Vagas abertas" indicador="100"></indicador>
            </div>

            <div class="col-4">
                <indicador titulo="Profissionais cadastrados" indicador="320"></indicador>
            </div>

            <div class="col-4">
                <indicador titulo="Visitantes online" indicador="15"></indicador>
            </div>
        </div>
    </div>
</template>
  
  
<script>
import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue';
import Indicador from '@/components/comuns/Indicador.vue';

export default {
    name: 'Home',
    components: {
        PesquisarVaga,
        Indicador
    }
}
</script>
  
  
<style></style>