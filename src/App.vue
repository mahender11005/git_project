<template>
  <div id="app">
    <prac_slot >
    <h1 slot="head1">  This is the line 1</h1>
    <h3 slot="head2"> this is the line 3</h3> 
      </prac_slot> <br />
    <div>
      <b-card no-body>
        <b-tabs pills card vertical>
          <b-tab title="HelloWorld"><HelloWorld /></b-tab>
          <b-tab title="About"><About /></b-tab>
          <b-tab title="countdown "><countdown /></b-tab>
          <b-tab title="Auto fill width "><mainInput /></b-tab>
          <b-tab title="custom_buttons " active><custom_buttons /></b-tab>
        </b-tabs>
      </b-card>
    </div>
  </div>
</template>

<script>
import About from "./components/About.vue";
import Countdown from "./components/countdown.vue";
import HelloWorld from "./components/HelloWorld.vue";
import mainInput from "./components/mainInput.vue";
import custom_buttons from "./components/custom_buttons.vue";
import prac_slot from "./components/prac_slot.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    About,
    Countdown,
    mainInput,
    custom_buttons,
    prac_slot,
  },
};
</script>

<style>
</style>
