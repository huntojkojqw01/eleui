<template>
  <div id="app">
    <p>{{ message }}</p>
    <el-button @click="visible = true" type="primary">Button</el-button>
    <el-dialog v-model="visible" title="Hello world">
      <p>Try Element</p>
    </el-dialog>
    <vtable></vtable>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      message: "Hello Vue!",
      visible: false
    }
  },
  components: ['vtable']
}
</script>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
  color: red;
}
</style>
