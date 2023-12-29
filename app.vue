<script setup lang="ts">
import VSvg from "./src/VSvg.vue"
</script>

<template>
  <div>
    <!-- name にファイル名（拡張子なし）を渡す -->
    <VSvg class="icon" name="home" />
    <VSvg class="icon" name="home" color="rgba(100, 200, 250, 0.8)" />
    <VSvg class="icon" name="good" color="red" />

    <hr />

    <img src="/home.svg" class="icon" />
    <img src="/good.svg" class="icon" />
  </div>
</template>

<style scoped>
.icon {
  width: 100px;
  height: 100px;
  margin: 10px;
}
</style>
