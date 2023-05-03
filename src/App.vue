
<script setup>
  import { ref } from 'vue';
  const count=ref(0);
</script>

<template>
  <main>
    <div>
      <h1>The current count is...</h1>
      <h1>{{ count }}</h1>
      <button @click=count-->-</button>
      <button @click=count++>+</button>
    </div>
  </main>
</template>

<style scope>
  main {
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  div {
    text-align: center;
  }

  button {
    width: 80px;
    height: 50px;
    margin: 10px;
    border-radius: 10px;
  }
</style>