<template>
    <h3>{{ texto }}</h3>

</template>

<script>
    export default{
        name: 'terceiroComponente',
        props: {
            texto: String
        }
    }
</script>


<style scoped>

    h3 {
        color: white;
        background-color: aqua;
        border-radius: 3px;
        margin: 0px 200px 0px 200px;
    }

</style>