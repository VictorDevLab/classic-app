<template>
  <p
    v-bind:class="{
      bold: true,
      italic: true,
      valid: isValid,
      invalid: !isValid,
    }"
  >
    Lorem ipsum dolor
  </p>
</template>

<script>
export default {
  data() {
    return {
      isValid: false,
    };
  },
};
</script>

<style>
.bold {
  font-weight: bolder;
}
.italic {
  font-style: italic;
}
.valid {
  color: forestgreen;
}
.invalid {
  color: orangered;
}
</style>
