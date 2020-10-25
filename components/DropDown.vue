<template>
  <div>
    <label for="countries">
      Select Country:
    </label>
    <select @change="dropDown(e)">
      <option value="US">US</option>
      <option value="KR">KR</option>
    </select>
  </div>
</template>

<script>
export default {
  methods: {
    dropDown(e) {
      console.log(e.target.value);
    }
  }
};
</script>

<style></style>
