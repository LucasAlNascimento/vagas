<template>
    <div class="container py-4">
        <div class="row">
            <div class="col">  
                <pesquisar-vaga></pesquisar-vaga>
            </div>
        </div>
        
        <div class="row mt-5">
            <div class="col-4">
                <div class="h-100 p-5 rounded-3 border bg-dark text-white">
                    <p>Vagas abertas</p>
                    <h2>18</h2>
                </div>
            </div>

            <div class="col-4">
                <div class="h-100 p-5 rounded-3 border bg-dark text-white">
                    <p>Profissionais cadastrados</p>
                    <h2>130</h2>
                </div>
            </div>

            <div class="col-4">
                <div class="h-100 p-5 rounded-3 border bg-dark text-white">
                    <p>Visitantes online</p>
                    <h2>10</h2>
                </div>
            </div>
        </div>
    </div>
</template>
  
  
<script>
import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue';

export default {
    name: 'Home',
    components: {
        PesquisarVaga
    }
}
</script>
  
  
<style></style>