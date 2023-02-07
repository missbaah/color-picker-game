<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script setup>
import useColorPicker from '../composables/color-picker';

const { colors, message, matchColor } = useColorPicker();


</script>

<style>

</style>
