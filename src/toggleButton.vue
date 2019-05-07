<template>
  <div>
    <button
      v-bind:class="{ selected: buttonSelected }"
      v-on:click="buttonSelected = !buttonSelected"
    >Toggle</button>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      buttonSelected: false
    };
  }
};
</script>
<style scoped>
button {
  padding: 10px 30px;
  background-color: #fff;
  border: 1px solid #ccc;
  border-radius: 5px;
  cursor: pointer;
  outline: 0;
}

button.selected {
  background-color: #6fa;
  border-color: #6fa;
}
</style>
