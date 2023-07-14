<template>
    <div class="menu-horizontal">
      <ul>
        <li><a href="#">Blog</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Description</a></li>
      </ul>
    </div>
  </template>
  
  <script>
import { defineComponent } from "vue";

export default defineComponent({
    name: 'MenuHorizontal'
});

</script>
  <style scoped>
  .menu-horizontal {
    background-color: rgb(79, 79, 243);
    padding: 10px;
  }
  
  .menu-horizontal ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
  }
  
  .menu-horizontal li {
    margin-right: 10px;
  }
  
  .menu-horizontal a {
    color: #f0eded;
    text-decoration: none;
    padding: 5px 10px;
  }
  
  .menu-horizontal a:hover {
    background-color: #333;
    color: #fff;
  }
  </style>
  