<template>
  <Container class="main d-flex flex-column justify-space-between align-center">
    <SocialMedia :isFooter="true" />
    <Contacts />
    <Logo />
  </Container>
  <Container
    v-if="$vuetify.display.mobile"
    class="copyright d-flex flex-column justify-space-between align-center"
  >
    <div class="copyright-text text-center">
      Copyright © 2025 FAEPEN/MT. Todos os Direitos Reservados.
    </div>
    <div class="mt-3">
      <v-img src="/assets/mrx.svg" width="120"></v-img>
    </div>
  </Container>
  <Container
    v-else
    class="copyright d-flex flex-row justify-space-between align-center"
  >
    <div class="copyright-text">
      Copyright © 2025 FAEPEN/MT. Todos os Direitos Reservados.
    </div>
    <div>
      <v-img src="/assets/mrx.svg" width="120"></v-img>
    </div>
  </Container>
</template>

<style scoped>
.main {
  background: rgb(51, 130, 74);
  background: linear-gradient(
    90deg,
    rgba(51, 130, 74, 1) 0%,
    rgba(74, 167, 101, 1) 100%
  );
}
.copyright-text {
  color: white;
}
.copyright {
  background-color: #16672e;
}
</style>
