<template>
  <div class="about">
    <h1>This is an about page</h1>
    <TComponent>
      <template v-slot:header="props">
        <p>header1 {{ props.junho }}</p>
      </template>
      <template #default>
        <p>body</p>
      </template>
    </TComponent>
  </div>
</template>

<script>
import TComponent from "@/components/TComponent.vue";
export default {
  components: {
    TComponent,
  },
};
</script>
