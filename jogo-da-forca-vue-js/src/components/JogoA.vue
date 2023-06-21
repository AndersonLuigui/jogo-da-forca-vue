<template>
    <div  class="jogo">
      
        <forca-a :erros="erros"/>

        <palavra-a 
        :palavra="palavra"
        :dica="dica"
        :verificarLetra="verificarLetra"
        :etapa="etapa"
        />

        <teclado-a
        v-if="etapa === 'jogo'"
        :letras="letras"
        :verificarLetra="verificarLetra"
        :jogar="jogar"
        />

        <final-a
        v-if="etapa != 'jogo'"
        :etapa="etapa"
        :texto="etapa === 'ganhador' ? 'Parabéns :)' : 'Não foi dessa vez'"
        :jogarNovamente="jogarNovamente"
        />

    </div>
</template>

<script>
import ForcaA from './ForcaA.vue'
import PalavraA from './PalavraA.vue'
import TecladoA from './TecladoA.vue'
import FinalA from './FinalA.vue'

export default {
    name: 'JogoA',
    props: {
        erros: Number,
        palavra: String,
        dica: String,
        verificarLetra: Function,
        etapa: String,
        letras: Array,
        jogar: Function,
        jogarNovamente: Function

    },
    data(){
        return{

        }
    },
    methods:{

    },
    components:{
        ForcaA,
        PalavraA,
        TecladoA,
        FinalA

    }

    

}
</script>

<style>
.jogo {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}


</style>