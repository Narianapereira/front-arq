<template>
  <main class="columns is-gapless is-multiline">
    <div class="container">
      <div class="flex-container">
        <div class="flex-item">
          <BarraSuperior />
        </div>
        <div class="flex-item">
          <BarraInferior :titulo="titulo" :itens="itens" class="barra-inferior"/>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import { defineComponent } from "vue";
import BarraSuperior from "./components/BarraSuperior.vue";
import BarraInferior from "./components/BarraInferior.vue";

export default defineComponent({
  name: "App",
  components: {
    BarraSuperior,
    BarraInferior,
  },
  data() {
    return {
      titulo: "Latest news",
      itens: [
        {
          subtitulo: "5 suggestions for frontend",
          texto: "Check-out some suggestions of how not to make a perfect frontend",
        },
        {
          subtitulo: "10 suggestions for backend",
          texto: "Learn how not make a disaster of a project",
        },
        {
          subtitulo: "From pharmacist to dev in 8 months",
          texto: "How to drop a career and start another when you get crazy",
        },
      ],
    };
  },
});
</script>

<style>
.container {
  display: flex;
  flex-direction: column;
  height: 100vh; /* Definindo altura total da tela */
}

.flex-container {
  flex: 1; /* Faz com que ocupe todo o espaço vertical disponível */
}

.flex-item {
  background-color: rgb(79, 79, 243);
  color: white;
  height: 50%; /* Define a altura para ocupar metade da tela */
}
.barra-inferior{
  background-color: white;
  text-align: center;
  padding: 20px;
}

</style>
