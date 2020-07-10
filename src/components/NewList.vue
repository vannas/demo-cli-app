<template>

<div id="main">
    <div class="lista card">
        <h2>Cosas Que Interesan a {{ Nombre }}</h2>

        <h4 v-if="Relevante=true">Áreas de Interés</h4>
        <ol>
            <li v-for="(Intereses, i) in Areas" v-bind:key="i"> {{i+1}}. {{Intereses}}</li>
        </ol>    
    </div>

</div>
    
</template>

<script>
export default {
    name: "NewList",
    el: "#main" ,
    data:function(){
        return {
            Nombre:'Verona',
            Relevante:true,
            msg: String,
            Areas:[
                'Coding', 
                'Diseño Gráfico',
                'Derechos Humanos', 
                'Trabajo Con Refugiados',   
                'Estudios de Género', 
                'Historia del Arte',
                'Artes Plásticas'
            ]
        }   
    }
}
</script>

<style scoped>

    #main {
        color:white;
        background-color: midnightblue;
    }

    h3 {
        color:lightsalmon;
    }

    li{
        list-style: none;
    }

</style>