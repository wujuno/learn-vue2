<template>
  <div>
    <h1>Learning Vue.js v2</h1>
    <TComponent title="Home title" name="Jh" />
  </div>
</template>

<script>
import TComponent from "@/components/TComponent.vue";
export default {
  data() {
    return {
      name: "Junho",
    };
  },
  components: {
    TComponent,
  },
};
</script>

<style scoped>
h1 {
  color: tomato;
  font-size: 3rem;
}
</style>
