<template>
  <div class="id">
    <button @click="$emit(togglelable)">{{label}}</button>
    <button @click="$emit(callback)">AlertBox</button>
  </div>
</template>

<script>
export default {
  name: "child",
  props: {
    label: String
  }
  //   methods: {
  //     callback: function(e) {
  //       this.$emit("click", e);
  //     },

  //     toggleLable: function(e) {
  //       this.$emit("click", e);
  //     }
  //   }
};
</script>

<style>
</style>