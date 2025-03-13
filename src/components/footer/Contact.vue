<template>
  <v-btn
    variant="text"
    color="white"
    class="contact-button text-none text-wrap text-center"
    height="auto"
    ><v-icon size="20">{{ icon }}</v-icon>
    <p class="text-wrap">{{ text }}</p></v-btn
  >
</template>

<script setup>
defineProps({
  text: String,
  icon: String,
});
</script>

<style>
.contact-button {
  font-size: 14px;
  font-weight: normal;
  padding: 10px !important;
}
</style>
