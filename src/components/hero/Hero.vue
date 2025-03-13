<template>
  <v-carousel
    v-if="$vuetify.display.mobile"
    hide-delimiters="true"
    :show-arrows="false"
    height="400"
    width="400"
  >
    <v-carousel-item src="/assets/banner-principal-mobile.png" cover>
    </v-carousel-item>
  </v-carousel>
  <v-carousel v-else hide-delimiters="true" :show-arrows="false" height="680">
    <v-carousel-item src="/assets/banner-principal.png" cover>
    </v-carousel-item>
  </v-carousel>
</template>

<script setup></script>
