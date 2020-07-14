<template>
  <button @click="$emit('onClick')" class="Button">{{label}}</button>
</template>

<script>
export default {
  name: "BaseButton",
  props: {
    label: {
      type: String,
      default: "Primary"
    }
  }
};
</script>

<style>
</style>