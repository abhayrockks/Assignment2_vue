<template>
  <div class="id">
    <base-button v-on:onClick="toggleLable" v-bind:label="label1"></base-button>
    <base-button @onClick="alertcallback" v-bind:label="'Alert'"></base-button>
  </div>
</template>

<script>
import BaseButton from "./Base-button.vue";
export default {
  name: "mainpage",
  components: {
    "base-button": BaseButton
  },

  data() {
    return {
      label1: "Primary"
    };
  },

  methods: {
    toggleLable() {
      if (this.label1 == "Primary") {
        this.label1 = this.label1.split("").reverse() .join("");
      } else {
        this.label1 = "Primary";
      }
    },
    alertcallback() {
      alert("Hi");
    }
  }
};
</script>

<style>
</style>