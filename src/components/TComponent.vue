<template>
  <div>
    <h2>{{ title }}</h2>
    <slot name="header" :junho="junho"></slot>
    <h1>body</h1>
    <slot></slot>
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
      junho: "coder",
    };
  },
  methods: {
    updateMsg() {
      this.msg = "Let's go !";
    },
  },
};
</script>
