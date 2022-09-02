<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <button class="button_one">Start Now</button>
      </div>
      <div class="col">
        <button class="button_three">Start Now</button>
      </div>
      <div class="col">
        <button class="button_two">Start Now</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "scss/_vars.scss";
.button_one {
  background-color: $Core_Green;
  color: $White;
  border: 0px;
  font-family: "Croma Sans";
  font-size: 35px;

  border-radius: 5px;
  font-weight: 450;
  padding-left: 15px;
  padding-right: 120px;
  text-align: left;
}
.button_two {
  background-color: $Core_Green;
  color: $White;
  border: 0px;
  font-family: "Croma Sans";
  font-size: 25px;

  border-radius: 5px;
  font-weight: 400;
  padding-left: 10px;
  padding-right: 90px;
  text-align: left;
}
.button_three {
  background-color: $Core_Green;
  color: $White;
  border: 0px;
  font-family: "Croma Sans";
  font-size: 30px;

  border-radius: 5px;
  font-weight: 450;
  padding-left: 12px;
  padding-right: 110px;
  text-align: left;
}
</style>