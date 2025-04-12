<template>
  <div class="d-flex flex-row justify-space-between social-media">
    <SocialMediaIcon
      icon="mdi mdi-instagram"
      link="https://www.instagram.com/faepenmt"
      :isFooter="isFooter"
    />
    <SocialMediaIcon icon="mdi mdi-facebook" :isFooter="isFooter" />
    <SocialMediaIcon icon="mdi mdi-youtube-tv" :isFooter="isFooter" />
  </div>
</template>

<script setup>
defineProps({
  isFooter: Boolean,
});
</script>
<style scoped>
.social-media {
  width: 130px;
  max-height: 24px;
}
</style>
