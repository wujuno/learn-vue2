<template>
  <div>
    <h2>{{ title }}</h2>
    <small>{{ name }}</small>
    <p>{{ msg }}</p>
    <button @click="updateMsg">Click here</button>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "default title",
    },
    name: {
      type: String,
    },
  },
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
