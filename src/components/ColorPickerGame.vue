<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script>
import { useColorPicker } from "../composables/color-picker";
// const { colors, message, matchColor } = useColorPicker();
export default {
  setup() {
    // return { colors, message, matchColor };
    return useColorPicker();
  },
};
</script>

<style></style>
