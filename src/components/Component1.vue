<template>
  <div class="id">
    <base-button v-on:onClick="toggleLable" v-bind:label="label"></base-button>
    <base-button @onClick="alertcallback" v-bind:label="'Alert'"></base-button>
  </div>
</template>

<script>
import BaseButton from "./Base-button.vue";
export default {
  name: "component1",
  components: {
    "base-button": BaseButton
  },

  data() {
    return {
      label: "Primary"
    };
  },

  methods: {
    toggleLable() {
      if (this.label == "Primary") {
        this.label = this.label.split("").reverse() .join("");
      } else {
        this.label = "Primary";
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
