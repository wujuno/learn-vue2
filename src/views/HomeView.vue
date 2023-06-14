<template>
  <div>
    <h1>This is Home page</h1>
    <form>
      <InputField v-model="name" />
      <br />
      <button>Submit</button>
    </form>
    {{ name }}
  </div>
</template>

<script>
import InputField from "@/components/InputField.vue";
export default {
  data() {
    return {
      name: "",
    };
  },
  components: {
    InputField,
  },
  methods: {
    updateName(name) {
      this.name = name;
    },
  },
};
</script>

<style scoped>
h1 {
  color: tomato;
  font-size: 3rem;
}
</style>
