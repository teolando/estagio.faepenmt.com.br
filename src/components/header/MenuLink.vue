<template>
  <div>
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
.active-link {
  color: #33824a;
}
</style>
