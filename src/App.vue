<template>
  <div id="app">
    <HelloWorld msg="Hello Vue in CodeSandbox!" />
    <ExampleChart />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ExampleChart from "./components/ExampleChart";

export default {
  name: "App",
  components: {
    HelloWorld,
    ExampleChart,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
