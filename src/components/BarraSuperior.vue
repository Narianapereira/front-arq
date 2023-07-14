<template>
    <div class="main-container">
      <div class="content-container">
        <menu-horizontal></menu-horizontal>
  
        <div class="custom-container">
          <div class="custom-left">
            <img src="../assets/cat2.jpg" alt="" class="dog">
          </div>
          <div class="custom-right">
            <h1 class="title">
              Nariana Pereira
            </h1>
            <h2 class="body">
              Currently I work as a backend software developer at CRM&Bônus, using technologies such as Java, MySQL, Docker and Kubernetes, solving bugs and developing new features.
              I'm a pharmacist who loves to study and be challenged. When I'm not coding or studying, you can find me outdoors rock climbing or hiking.
            </h2>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { defineComponent } from "vue";
  import MenuHorizontal from "./MenuHorizontal.vue";
  
  export default defineComponent({
    name: "BarraSuperior",
    components: {
      MenuHorizontal
    }
  });
  </script>
  
  <style scoped>
  .main-container {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .content-container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .title {
    color: #fcfafa;
  }
  
  .body {
    text-align: justify;
  }
  
  .dog {
    border-radius: 50%;
  width: 40%;
  height: auto;
  }
  
  .custom-container {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
    margin-right: 30%;
    width: 80%;

  }
  
  .custom-left {
    text-align: right;
    padding-right: 10px;
    flex-basis: 65%;
  }
  
  .custom-right {
    text-align: left;
    padding-left: 10px;
    flex-basis: 55%;
  }
  </style>
  