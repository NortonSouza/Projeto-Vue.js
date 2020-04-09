<template>
    <div id="app" style="">


        <!-- routes will be rendered here -->

        <div style="margin-bottom:100px;">
            <Gerador />
        </div>

        <div id="conversores">
            <h1 class="tituloCentro">Conversor de Moedas</h1>
            <div class="linha">
                <Conversor moeda-a="USD" moeda-b="BRL" />
                <Conversor moeda-a="BRL" moeda-b="USD" />
            </div>
            <div class="linha">
                <Conversor moeda-a="CAD" moeda-b="BRL" />
                <Conversor moeda-a="BRL" moeda-b="CAD" />
            </div>
            <div class="linha">
                <Conversor moeda-a="EUR" moeda-b="BRL" />
                <Conversor moeda-a="BRL" moeda-b="EUR" />
            </div>

        </div>
    </div>
</template>

<script>

    import Conversor from "./components/Conversor.vue";
    import Gerador from "./components/middle.vue";


    export default {
        name: 'App',
        components: {
            Conversor,
            Gerador
            //Header
        }
    }
</script>

<style>

    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        /*-webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;*/
        /*text-align: center;*/
        color: #2c3e50;
        /*margin-top: 60px;*/
    }

    .linha {
        margin-top: 40px;
        display: flex;
        justify-content: space-around;
    }

    .tituloCentro {
        text-align: center;
    }
</style>
