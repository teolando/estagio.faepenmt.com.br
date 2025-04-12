<template>
  <a :href="link" target="_blank">
    <v-hover v-if="!isFooter">
      <template v-slot:default="{ isHovering, props }">
        <v-icon
          :icon="icon"
          size="30"
          v-bind="props"
          :style="{
            'color': isHovering ? '#33824A' : '#525252',
          }"
        />
      </template>
    </v-hover>
    <v-hover v-if="isFooter">
      <template v-slot:default="{ isHovering, props }">
        <v-icon
          :icon="icon"
          size="24"
          v-bind="props"
          :style="{
            'color': isHovering ? '#525252' : 'white',
          }"
        />
      </template>
    </v-hover>
  </a>
</template>

<script setup>
defineProps({
  icon: String,
  isFooter: Boolean,
  link: String,
});
</script>
