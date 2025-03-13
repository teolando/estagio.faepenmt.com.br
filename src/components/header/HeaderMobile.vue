<template>
  <div class="d-flex flex-row justify-space-around align-center main">
    <div>
      <Logo />
    </div>

    <div class="d-flex flex-column justify-center align-end">
      <slot></slot>
    </div>
  </div>
</template>
<script setup></script>
<style scoped>
.main {
  height: 120px;
}
</style>
