<template>
    <div  class="palavra">

        <div class="palavra-letras">

            <div class="palavra-letra" v-for="{letra,key} in palavra" :key="key">
                {{ letra }}

            </div>

        </div>

        <div class="palavra-dica">
            {{ dica }}
        </div>

    </div>
</template>

<script>


export default {
    name: 'PalavraA',
    props: {
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

    }

}
</script>

<style>
    .palavras{
        text-transform: uppercase;
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
    }

</style>