<template>
  <child v-on:togglelable="togglelable()" v-on:callback="callback()" :label.sync="label"></child>
</template>

<script>
import child from "./Child.vue";
export default {
  name: "Button",
  components: {
    child
  },
  data() {
    return {
      label: "Primary"
    };
  },

  methods: {
    togglelable: function() {
      if (this.label == "Primary") {
        this.label = this.label.split("").reverse().join("");
      } else {
        this.label = "Primary";
      }
    },
    callback: function() {
      alert("Hi");
    }
  }
};
</script>

<style>
button {
  padding: 10px 20px;
  border: 1px solid #ddd;
  color: rgb(240, 221, 221);
  background-color: rgb(49, 103, 204);
  border-radius: 4px;
  font-size: 14px;
  cursor: pointer;
}
</style>