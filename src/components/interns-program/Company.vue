<template>
  <v-col cols="4" class="col pb-10">
    <div class="d-flex flex-column justify-center align-center main">
      <v-img :src="image" class="image"> </v-img>
      <p class="title">
        {{ title }}
      </p>
      <v-hover>
        <template v-slot:default="{ isHovering, props }">
          <v-btn
            height="44"
            v-bind="props"
            :href="to"
            class="button text-capitalize"
            :style="{ 'background-color': isHovering ? '#33824A' : '#525252' }"
            >Ver Vagas</v-btn
          >
        </template>
      </v-hover>
    </div>
  </v-col>
</template>
<script setup>
defineProps({
  image: String,
  title: String,
  to: String,
});
</script>
<style scoped>
.image {
  width: 300px;
  height: 300px;
  border: 1px solid #33824a;
  border-radius: 40px;
}

.col {
  margin: 0;
}
.title {
  color: #525252;
  font-size: 28px;
  text-align: center;
}
.button {
  color: white;
  font-size: 28px;
  font-weight: bold;
  line-height: auto;
  letter-spacing: 1px;
  padding: 0px 30px;
  border-radius: 10px;
}
</style>
