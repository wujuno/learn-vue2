<template>
  <div>
    <h1>Learning Vue.js v2</h1>
    <change-btn></change-btn>
  </div>
</template>

<script>
import ChangeBtn from "@/components/ChangeBtn.vue";
export default {
  data() {
    return {
      name: "Junho",
    };
  },
  components: {
    ChangeBtn,
  },
};
</script>

<style scoped>
h1 {
  color: tomato;
  font-size: 3rem;
}
</style>

ChangeBtn
