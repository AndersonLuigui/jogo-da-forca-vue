<template>
    <div  class="jogo">
      
        <forca-a :erros="erros"/>
        <palavra-a 
        :palavra="palavra"
        :dica="dica"/>

    </div>
</template>

<script>
import ForcaA from './ForcaA.vue'
import PalavraA from './PalavraA.vue'

export default {
    name: 'JogoA',
    props: {
        erros: Number,
        palavra: String,
        dica: String

    },
    data(){
        return{

        }
    },
    methods:{

    },
    components:{
        ForcaA,
        PalavraA

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