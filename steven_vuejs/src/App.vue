<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!--   <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <button @click="onSuppliersListClick()">Suppliers</button>
    <button @click="onMapClick()">Map</button>
    <SuppliersList/>
    <SuppliersMap/>
</template>

<script>
/* import HelloWorld from "./components/HelloWorld.vue"; */
import SuppliersList from "./components/SuppliersList.vue";
import SuppliersMap from "./components/SuppliersMap.vue";
export default {
  name: "App",
  components: {
/*     HelloWorld, */
    SuppliersList,
    SuppliersMap,
  },
  methods: {
    onSuppliersListClick: () => {
      window.alert("supplierslist");
    },
    onMapClick: () => {
      window.alert("suppliersmap");
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
