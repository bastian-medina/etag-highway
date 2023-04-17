<template>
      <q-header elevated style="background-color: #a6aec1;">
        <q-toolbar dense align="justify">
          <q-toolbar-title >E-TAG servicios integrales.</q-toolbar-title>
        </q-toolbar>

        <q-tabs v-model="tab">
          <q-tab name="inicio" label="Inicio" @click="goToIndex()" />
          <q-tab name="servicios" label="Servicios" to="/services" @click="goToServices()" />
          <q-tab name="sobreNosotros" label="Sobre Nosotros" to="/aboutUs" @click="goToAboutUs()" />
          <q-tab name="contactanos" label="Contactanos" to="/contactUs" @click="goToContactUs()" />
        </q-tabs>
      </q-header>
</template>

<script setup>
import { ref } from 'vue'
import { useRoute, useRouter } from "vue-router";

//variables
const tab = ref('inicio')
const route = useRoute();
const router = useRouter();


//methods
const goToIndex = () => {
    router.push("/");
};

const goToServices = () => {
    router.push("/services");
};

const goToAboutUs = () => {
    router.push("/aboutUs");
};

const goToContactUs = () => {
    router.push("/contactUs");
};
</script>

<style>
.text-black {
  color: #000000;
}
</style>