<template>
  <div>
    <p>{{ msg }}</p>
    <button @click="updateMsg">Click here</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Ready to Learning?",
    };
  },
  methods: {
    updateMsg() {
      this.msg = "Let's go !";
    },
  },
};
</script>
