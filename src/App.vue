<template>
  <div id="app">
    <div>
      <b-card no-body>
        <b-tabs pills card vertical>
          <b-tab title="HelloWorld" active><HelloWorld /></b-tab>
          <b-tab title="About"><About /></b-tab>
        </b-tabs>
      </b-card>
    </div>
  </div>
</template>

<script>
import About from "./components/About.vue";
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    About,
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
