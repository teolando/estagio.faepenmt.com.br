<template>
  <v-carousel
    v-if="$vuetify.display.mobile"
    hide-delimiters="true"
    :show-arrows="false"
    height="400"
    width="400"
  >
    <v-carousel-item src="/assets/banner-principal-mobile.png" cover>
      <div class="d-flex flex-column align-center justify-center image-hero">
        <div class="d-flex flex-column">
          <div class="text-h4 text-left text-white px-5">Conectando Estudantes, Empresas e Instituições de ensino</div>
          <div class="text-h6 text-left text-white px-5 subtitle">Somos agente integrador de Estágio</div>
        </div>
        <v-hover>
        <template v-slot:default="{ isHovering, props }">
          <v-btn
            height="44"
            v-bind="props"
            :href="to"
            class="button-hero text-capitalize mt-5"
            :style="{ 'background-color': isHovering ? '#33824A' : '#33824A' }"
            >Ver Vagas</v-btn
          >
        </template>
      </v-hover>
      <v-hover>
        <template v-slot:default="{ isHovering, props }">
          <v-btn
            height="44"
            v-bind="props"
            :href="to"
            class="button-hero text-capitalize mt-3"
            :style="{ 'background-color': isHovering ? '#33824A' : '#525252' }"
            >Sou empresa</v-btn
          >
        </template>
      </v-hover>
      </div>
    </v-carousel-item>
  </v-carousel>
  <v-carousel v-else hide-delimiters="true" :show-arrows="false" height="680">
    <v-carousel-item src="/assets/banner-principal.png" cover>
    </v-carousel-item>
  </v-carousel>
</template>

<script setup></script>

<style>
.subtitle {
  font-weight: normal;
}
.image-hero {
  height: 100%;
  background-color: rgba(26, 73, 39, 0.3);
}
.button-hero {
  color: white;
  font-size: 20px;
  font-weight: bold;
  line-height: auto;
  letter-spacing: 1px;
  padding: 0px 30px;
  border-radius: 10px;
}
</style>
