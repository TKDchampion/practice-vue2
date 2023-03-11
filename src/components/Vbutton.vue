<template>
  <div>
    <button @click="increment">{{ count }}</button>
  </div>
</template>

<script>
import { ref } from "vue-demi";

export default {
  name: "VButton",
  //   setup() {
  //     const count = ref(0);

  //     const increment = () => {
  //       count.value++;
  //       console.log(count.value);
  //     };

  //     return {
  //       count,
  //       increment,
  //     };
  //   },
  data() {
    return { count: 0 };
  },
  methods: {
    increment() {
      this.count++;
      console.log(this.count);
    },
  },
};
</script>
