<template>
  <div v-if="$vuetify.display.mobile">
    <v-img src="/assets/logo.png" width="200px" height="50"></v-img>
  </div>
  <div v-else>
    <v-img src="/assets/logo.png" width="263" height="80"></v-img>
  </div>
</template>

<script setup></script>
