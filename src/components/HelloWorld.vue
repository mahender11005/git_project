<template>
  <div class="container pb-3 ">
    <div class="row">
      <h1 class="text-center pb-2">Personel Information</h1>
      <div class="col-12 div-border">
        <form action="">
          <label for=""><b>village: </b> </label
          ><input
            type="text"
            v-model="infom.vill"
            class="full-width borderr"
            placeholder="Enter your village"
          />
          <br />
          <br />
          <label><b>mandal: </b> </label
          ><input
            type="text"
            v-model="infom.mandal"
            class="full-width"
            placeholder="Enter your mandal"
          />
          <br />
          <br />
          <label> <b> district: </b> </label
          ><input
            type="text"
            v-model="infom.dist"
            class="full-width"
            placeholder="Enter your district"
          />
          <br />
          <br />
          <label> <b> Pin number : </b> </label>
          <select v-model="infom" class="full-width">
            <option v-for="(x, i) in value" :value="x" v-bind:key="i">
              {{ x.pin }}
            </option>
          </select>
        </form>
      </div>

      <div class="mt-3 text-center">
        <table class="table table-bordered">
          <thead>
            <tr>
              <th>Village</th>
              <th >Pin code</th>
              <th>Mandal</th>
              <th>District</th>
            </tr>
          </thead>
          <tbody>
           
            <tr v-for="(x,i) in change" v-bind:key="i" >
              <td>{{ x.vill }}</td>
              <td>{{ x.pin }}</td>
              <td>{{ x.mandal }}</td>
              <td>{{ x.dist }}</td>
            </tr>

              <tr>
              <td></td>
              <td>SUM : {{sum}}</td>
              <td></td>
              <td></td>
            </tr>

          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      infom: "",
      change:[],
      tablee:"",
      sum:0,
      value: [
        {
          vill: "jammikunta",
          pin: 505122,
          mandal: "jammikunta",
          dist: "karimnagar",
        },
        {
          vill: "huzurabad",
          pin: 505123,
          mandal: "dubbaka",
          dist: "karimnagar",
        },
        {
          vill: "jagital",
          pin: 505124,
          mandal: "kondagattu",
          dist: "rajanna jilla",
        },
        {
          vill: "warangal",
          pin: 505125,
          mandal: "hanumakonda",
          dist: "warangal",
        },
      ],
    };
  },
  watch: {
    infom(newValue) {
      console.log(newValue.pin);
      this.change.push(newValue)
      this.sum=this.sum+newValue.pin
      
   
     
    },
  },
};
</script>

<style lang="scss" scoped>
$color-te: rgb(123, 88, 39);
.full-width {
  width: 100%;
  padding: 5px;
  display: inline-block;
  border: 2px solid #ccc;
  border-radius: 5px;
  box-sizing: border-box;
  cursor: pointer;
}
select:hover {
  background-color: rgb(115, 111, 111);
  color: white;
}
.div-border {
  border: 0.01px solid;
  padding: 20px;
  border-radius: 10px;
  background-color: #f2f2f2;
}
</style>