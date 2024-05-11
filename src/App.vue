<template>
  <p v-for="user in legalUsers" :key="user.name">{{ user.name }}</p>
</template>

<script>
export default {
  data() {
    return {
      users: [
        { name: "John", age: 33 },
        { name: "Jane", age: 33 },
        { name: "Jack", age: 17 },
        { name: "Jill", age: 16 },
      ],
    };
  },
  computed: {
    legalUsers() {
      return this.users.filter((user) => user.age >= 18);
    },
  },
};
</script>

<style>
div {
  background-color: rgb(132, 118, 118);
  border: 2px solid white;
}

p {
  background-color: rgb(124, 98, 149);
}
</style>
