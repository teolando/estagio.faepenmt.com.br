<template>
  <v-col lg="auto" md="auto" sm="12" class="col pb-10">
    <div class="d-flex flex-column justify-center align-center main">
      <img v-bind="props" :src="image" class="image" />
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
            :style="{
              'background-color': isHovering ? '#33824A' : '#525252',
            }"
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
  width: 360px;
  height: 360px;
  border: 2px solid #525252;
  border-radius: 40px;
}

.col {
  margin: 0;
}
.title {
  color: #525252;
  font-size: 20px;
  text-align: center;
}
.button {
  color: white;
  font-size: 20px;
  font-weight: bold;
  line-height: auto;
  letter-spacing: 1px;
  padding: 0px 30px;
  border-radius: 10px;
}
</style>
