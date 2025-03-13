<template>
  <v-col
    class="d-flex justify-center align-center"
    cols="12"
    sm="12"
    xs="12"
    md=""
  >
    <div class="d-flex flex-column justify-center align-center">
      <v-img :src="image" class="image"></v-img><TitleBenefit :title="title" />
    </div>
  </v-col>
</template>

<script setup>
defineProps({
  title: String,
  image: String,
});
</script>
<style>
.image {
  width: 120px;
}
</style>
