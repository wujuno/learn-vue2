<template>
  <div>
    <h1>This is Home page</h1>
    <form action="">
      <label for="">Name </label>
      <input
        type="text"
        :value="value"
        @input="$emit('input', $event.target.value)"
      />
    </form>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      required: true,
    },
  },
  /* methods: {
    updateName(e) {
      this.$emit("update-name", e.target.value);
    },
  }, */
};
</script>
