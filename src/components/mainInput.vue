<template>
  <div class="container-fluid bg-main">
    <h1 class="pb-2">Auto fill width</h1>
    <div class="row pb-2">
      <div class="col">
        <custom-input class="w-100" />
      </div>
      <div class="col">
        <custom-input class="w-100" />
      </div>
    </div>
    <div class="row pb-2">
      <div class="col">
        <custom-input class="w-100" />
      </div>
    </div>
    <div class="row pb-2">
      <div class="col">
        <custom-input class="w-100" />
      </div>
      <div class="col">
        <custom-input class="w-100" />
      </div>
      <div class="col">
        <custom-input class="w-100" />
      </div>
    </div>
  </div>
</template>

<script>
import customInput from "./customInput.vue";
export default {
  components: { customInput },
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.bg-main {
  border: 1px solid rgb(132, 131, 131);
  padding: 10px;
  border-radius: 5px;
  background-color: rgb(245, 239, 231);
    text-align: center;
  color: #2c3e50;
}
</style>
