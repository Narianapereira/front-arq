<template>
    <div>
      <h1 class="title">{{ titulo }}</h1>
      <div class="content">
      <div v-for="(item, index) in itens" :key="index" class="item">
        <h2 class="subtitle">{{ item.subtitulo }}</h2>
        <p class="text">{{ item.texto }}</p>
      </div>
      </div>
    </div>
  </template>
  
  <script>
  import { defineComponent } from "vue";
  
  export default defineComponent({
    name: "MeuComponente",
    props: {
      titulo: {
        type: String,
        required: true,
      },
      itens: {
        type: Array,
        required: true,
      },
    },
  });
  </script>
  
  <style scoped>
  .title {
    color: #4737a5;
    font-size: 20px;
    font-weight: bold;
  }
  
  .subtitle {
    color: #514886;
    font-size: 16px;
    font-weight: bold;
    margin-bottom: 5px;
  }
  
  .item {
    margin-bottom: 20px;
    color: #514886;
  }
  .text {
  color: #514886;
  font-size: 12px;
  justify-content: center;
}
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
  </style>
  