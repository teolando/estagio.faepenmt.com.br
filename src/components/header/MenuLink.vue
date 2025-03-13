<template>
  <div v-if="$vuetify.display.mobile">
    <router-link :to="to" class="mobile">{{ title }}</router-link>
  </div>
  <div v-else>
    <router-link :to="to" class="main">{{ title }}</router-link>
  </div>
</template>
<script setup>
defineProps({
  to: String,
  title: String,
});
</script>

<style scoped>
.main {
  text-decoration: none;
  color: #666666;
  text-align: end;
  width: min-content;
  font-weight: 300;
  font-size: 18px;
}

.mobile {
  text-decoration: none;
  color: #666666;
  text-align: end;
  width: min-content;
  font-weight: 300;
  font-size: 22px;
  letter-spacing: 2px;
  height: 50px;
}
.active-link {
  color: #33824a;
}
</style>
