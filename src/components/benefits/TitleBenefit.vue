<template>
  <p class="title">{{ title }}</p>
</template>
<script setup>
defineProps({
  title: String,
});
</script>

<style scoped>
.title {
  color: #33824a;
  font-size: 18px;
  font-weight: 700;
  text-align: center;
}
</style>
