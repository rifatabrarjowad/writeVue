import InputText from "primevue/inputtext";

<template>
  <div>
    <InputText v-model="text" />
    <Button label="greet" icon="pi pi-user" @click="greet" />
    <br />
    <br />
    <textarea
      disabled
      name=""
      id=""
      cols="50"
      v-model="text"
      rows="7"
      style="font-size: 35px; border: 5px solid"
    ></textarea>
    <Toast />
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: null,
    };
  },
  methods: {
    greet() {
      this.$toast.add({
        severity: "info",
        summary: "sorry ☹",
        detail: "this is not available ",
      });
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>