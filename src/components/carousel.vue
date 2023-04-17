<template>
      <q-carousel
        animated
        infinite
        swipeable
        arrows
        v-model="slide"
        height="460px"
        :autoplay="autoplay"
        transition-prev="slide-right"
        transition-next="slide-left"
        @mouseenter="autoplay = false"
        @mouseleave="autoplay = true"
      >
        <q-carousel-slide :name="3" img-src="https://i.ibb.co/z404q6W/aseo.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Administradora De Servicios Integrales</div>
            <div class="text-subtitle1">Somos profesionales en aseo y limpieza y buscamos entregar cada uno de nuestros servicios con atención de eficiencia y calidad enfocada en las necesidades de nuestros clientes.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="2" img-src="https://i.ibb.co/9yHtm62/aseo-profundo.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Aseo industrial</div>
            <div class="text-subtitle1">Somos profesionales en aseo y limpieza y buscamos entregar cada uno de nuestros servicios con atención de eficiencia y calidad enfocada en las necesidades de nuestros clientes.</div>
          </div>
        </q-carousel-slide>
        
        <q-carousel-slide :name="1" img-src="https://i.ibb.co/3SdMnS8/interior-aseo.png">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Administradora De Servicios Integrales</div>
            <div class="text-subtitle1">Somos profesionales en aseo y limpieza y buscamos entregar cada uno de nuestros servicios con atención de eficiencia y calidad enfocada en las necesidades de nuestros clientes.Somos profesionales en aseo y limpieza y buscamos entregar cada uno de nuestros servicios con atención de eficiencia y calidad enfocada en las necesidades de nuestros clientes.</div>
          </div>
        </q-carousel-slide>
        
      </q-carousel>
  </template>
  
<script setup>
import { ref } from 'vue'
  
const slide = ref(1)
const autoplay = ref(true)
</script>

<style lang="sass" scoped>
.custom-caption
  text-align: center
  padding: 12px
  color: white
  background-color: rgba(0, 0, 0, .3)
</style>
