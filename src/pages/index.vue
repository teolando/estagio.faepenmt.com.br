<template>
  <v-layout>
    <v-navigation-drawer v-model="drawer" temporary>
      <v-list-item>
        <Logo />
      </v-list-item>

      <v-divider></v-divider>
      <div class="d-flex flex-column align-center justify-center">
        <MenuLink to="/" title="Home" />
        <MenuLink to="/sobre" title="Sobre" />
        <MenuLink to="/vagas" title="Vagas" />
        <MenuLink to="/contato" title="Contato" />
      </div>
      <v-divider></v-divider>
      <div class="d-flex flex-row align-center justify-center">
        <SocialMedia class="mt-4" />
      </div>
    </v-navigation-drawer>
    <v-main>
      <div>
        <HeaderMobile v-if="$vuetify.display.mobile">
          <div class="d-flex justify-center align-center h-100">
            <v-btn
              icon
              variant="text"
              color="#525252"
              @click.stop="drawer = !drawer"
            >
              <v-icon size="40">mdi mdi-menu</v-icon>
            </v-btn>
          </div></HeaderMobile
        >
        <Header v-else />
      </div>
      <Hero />
      <InternsProgram />
      <About />
      <Benefits />
      <Footer />
    </v-main>
  </v-layout>
</template>

<script setup>
//
import { ref } from "vue";

const drawer = ref(null);
</script>
