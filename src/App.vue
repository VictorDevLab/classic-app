<template>
  <p v-for="(name, idx) in names" :key="name.id">
    {{ idx }} {{ name.first }} {{ name.last }}
  </p>
</template>

<script>
export default {
  data() {
    return {
      names: [
        { id: 0, first: "John", last: "Doe" },
        { id: 1, first: "Jane", last: "Doe" },
      ],
    };
  },
};
</script>
