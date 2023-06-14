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
  components: {
    InputField,
  },
  data() {
    return {
      name: "antlinesoft developer",
    };
  },
  beforeCreate() {
    //인스턴스 생성 되기 전에는 데이터 접근 불가능
    console.log("beforeCreate", this.name);
  },
  created() {
    //여기서부터 데이터 접근 가능
    //보통 서버로 요청을 보낸다.
    console.log("created", this.name);
  },
  beforeMount() {
    alert("beforeMount");
  },
  mounted() {
    //여기서부터 DOM에 접근 가능
    alert("mounted");
  },
  beforeUpdate() {
    alert("beforeUpdate");
  },
  updated() {
    // DOM 변환이 일어남
    alert("updated");
  },
  beforeDestroy() {
    alert("beforeDestroy");
  },
  destroyed() {
    // 메모리 누수를 방지하기 위해 이벤트리스너를 삭제하던지
    // 데이터를 초기화하는 작업들을 할 수 있다.
    alert("destroyed");
  },
};
</script>

<style scoped>
h1 {
  color: tomato;
  font-size: 3rem;
}
</style>
