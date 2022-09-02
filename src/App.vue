<template>
  <div id="app">
    <div>
      <b-card no-body>
        <b-tabs pills card vertical>
          <b-tab title="HelloWorld"><HelloWorld /></b-tab>
          <b-tab title="About"><About /></b-tab>
           <b-tab title="countdown " ><countdown  /></b-tab>
             <b-tab title="Auto fill width " ><mainInput  /></b-tab>
              <b-tab title="custom_buttons "   active><custom_buttons  /></b-tab>
       
          
        </b-tabs>
      </b-card>
    </div>
  </div>
</template>

<script>
import About from "./components/About.vue";
import Countdown from './components/countdown.vue';
import HelloWorld from "./components/HelloWorld.vue";
import mainInput from "./components/mainInput.vue";
import custom_buttons from "./components/custom_buttons.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    About,
    Countdown,
    mainInput,
    custom_buttons,
  },
};
</script>

<style>


</style>
