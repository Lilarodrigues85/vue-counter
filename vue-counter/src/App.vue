<template>
  <div id="app">
    <h1>Contador: {{ count }}</h1>
    <button @click="increment">Aumentar</button>
    <button @click="decrement">Diminuir</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
  },
};
</script>

<style>
#app {
  text-align: center;
  margin-top: 50px;
}
button {
  margin: 5px;
  padding: 10px;
  font-size: 16px;
  cursor: pointer;
}
</style>
