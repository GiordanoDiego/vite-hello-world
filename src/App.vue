<script>
/*
    utilizzare un componente dentro un altro
    1) importazione del componente
    2) dichiarazione del componente all'interno dell'oggetto
    3) utilizzo del componente
*/

// 1) importazione
import AppHeader from './components/AppHeader.vue';
    export default {
        data() {
            return { 
                count: 0 
            }
        },
        // 2) Dichiaro il componente
        components:{
            AppHeader
        }
    }
</script>

<template>
    <div>
        <!--3 step dichiarano il componente avremo un tag che corrisponde al nostro componente
            e quindi sparera al posto del componente il codice contenten nel componente
        -->
        <AppHeader/> 
        <!-- qui scriverà il codice del componente -->
        <p>
            {{ count }}
        </p>
    </div>
    <button @click="count++">
        Incrementa
    </button>
  
</template>

<style scoped>

</style>
