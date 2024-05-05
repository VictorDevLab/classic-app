<template>
  <!-- <p>{{ thisInArrowFunc() }}</p> -->
  <p>{{ username }}</p>
  <button @click="changeName('whasdrdt')">Change Name</button>
</template>

<script>
export default {
  data() {
    return {
      username: "Obi-Wan Kenobi",
    };
  },
  methods: {
    changeName(name) {
      this.username = name;
    },
  },
};
</script>
