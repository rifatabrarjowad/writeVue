<template>
  <div>
    <Editor v-model="value2" editorStyle="height: 320px">
      <template v-slot:toolbar>
        <span class="ql-formats">
          <button class="ql-bold" v-tooltip.bottom="'Bold'"></button>
          <button class="ql-italic" v-tooltip.bottom="'Italic'"></button>
          <button class="ql-underline" v-tooltip.bottom="'Underline'"></button>
        </span>
      </template>
    </Editor>
  </div>
</template>

<script>
export default {
  
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
