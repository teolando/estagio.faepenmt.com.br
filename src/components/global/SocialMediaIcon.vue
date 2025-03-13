<template>
  <a :href="link">
    <v-icon :icon="icon" size="24" :color="isFooter ? 'white' : '#33824A'" />
  </a>
</template>

<script setup>
defineProps({
  icon: String,
  isFooter: Boolean,
  link: String,
});
</script>
