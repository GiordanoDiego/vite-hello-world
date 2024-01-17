<script>
    export default {
        data() {
            return { 
                title: 'ciao ragazzi'
            }
        },
    }
</script>

<template>
    <header>
        <h1>
            {{ title }}
        </h1>
    </header>
  
</template>

<style scoped> /* qui ci vanno le classi che sono visibili solo a questo componente*/
    h1{
        color:brown;
        text-align: center;
        background-color: aquamarine;
    }
</style>
