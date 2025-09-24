<script>
export default {
  data() {
    return {
      contador: 0
    }
  },
  methods: {
    saludar() {
      console.log("hola")
    }
    , incrementar(){
      this.contador++;
    },
    restar(){
      this.contador--;
    },
    resetV(){
      this.contador = 0;
    }
  }
}
</script>

<template>
  <img src="./assets/logo.svg" alt="logo vue" width="125px" height="125px">
  <h1>Hola mundo desde Vue js 3</h1>

  <hr />

  <h2>contador: {{ contador }}</h2>

  <button @click="incrementar()">+1</button>
  <button @click="restar()">-1</button>
  <button @click="resetV()">reset</button>
</template>

<style scoped>  
h1 {
  color: yellow;
}
</style>
