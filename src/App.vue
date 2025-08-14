<template>
  <div class="w-1/2 mx-auto p-4">
    <div>Name: {{ person.name }}</div>
    <div>Second name: {{ person.secondName }}</div>
    <div>Age: {{ person.age }}</div>
    <div>
      <span @click="sayOne(123)" class="text-xl font-bold cursor-pointer">Click</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Our App",
  data() {
    return {
      person: {
        name: "Ivan",
        secondName: "Ivanov",
        age: 20,
      },
    };
  },
  methods: {
    sayOne(num) {
      console.log(num);
    },
  },
};
</script>

<style scoped></style>
