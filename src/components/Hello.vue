<template>
  <div>
    <h1>Hello , I'm {{ name }}</h1>
    <el-radio v-model="radio" label="1">Option A</el-radio>
    <el-radio v-model="radio" label="2">Option B</el-radio>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "Hello",
      radio: "2",
    };
  },
};
</script>

<style>
</style>