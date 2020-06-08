<template>
  <div id="app">
    <div>
      <h1>Compara el Clima</h1>
    </div>
    <b-container fluid class="bv-example-row">
      <b-row>
        <b-col sm="5" md="6"> <Origen msg="Ciudad de Origen"/></b-col>
        <b-col sm="5" offset-sm="2" md="6" offset-md="0">
          <Destino msg="Ciudad Destino"
        /></b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Destino from "./components/Destino";
import Origen from "./components/Origen";

export default {
  name: "App",
  components: {
    Destino,
    Origen,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
body {
  font-family: "montserrat", sans-serif;
}
#app {
  top: auto;
  text-align: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #eeeeee;
  color: #444444;
  box-sizing: border-box;
}
h1 {
  padding: 6%;
}
</style>
