<template>
  <div id="app">
    <div>
      <b-card no-body>
        <b-tabs pills card vertical>
          <b-tab title="HelloWorld"><HelloWorld /></b-tab>
          <b-tab title="About"  active><About /></b-tab>
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

</style>
