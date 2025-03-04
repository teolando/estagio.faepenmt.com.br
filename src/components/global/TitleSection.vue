<template>
  <h3 class="title" :style="'color:' + color + ';'">{{ title }}</h3>
</template>
<script setup>
defineProps({
  color: String,
  title: String,
});
</script>

<style scoped>
.title {
  font-size: 40px;
  font-weight: 900;
  text-align: center;
}
</style>
