
<!-- <script setup>
  import { ref } from 'vue';
  const count=ref(0);

  const addToCount=()=>{
    count.value++
  }

  const subFromCount=()=>{
    count.value--
  }

</script> -->

<script>
export default (
  {
    data() {
      return {
        count: 0
      }
    },
    methods: {
      addToCount() {
        this.count++
      },
      subFromCount() {
        this.count--
      }
    },
  }
)
</script>

<template>
  <main>
    <div>
      <h1>The current count is...</h1>
      <h1>{{ count }}</h1>
      <button @click="subFromCount">-</button>
      <button @click="addToCount">+</button>
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