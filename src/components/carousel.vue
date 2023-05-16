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
        <q-carousel-slide :name="6" img-src="https://www.lyms.net/wp-content/uploads/2016/01/limpieza-oficinas-Zaragoza.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Aseo de oficinas</div>
            <div class="text-subtitle1">Los servicios de oficina proporcionan soluciones profesionales y eficientes para la gestión de tareas administrativas y el mantenimiento de un espacio de trabajo productivo y organizado.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="6" img-src="https://cleancontrol.es/wp-content/uploads/2021/02/conserjeria-min-1024x589.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Servicios de conserjeria</div>
            <div class="text-subtitle1">Los servicios de conserjería proporcionan una atención personalizada y soluciones rápidas a problemas cotidianos en edificios y complejos residenciales, mejorando la calidad de vida de los residentes.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="5" img-src="https://equipamientoyseguridad.com/wp-content/uploads/instalacion-camaras-de-vigilancia-negocio.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Servicios de vigilancia</div>
            <div class="text-subtitle1">Los servicios de vigilancia garantizan la seguridad y previenen incidentes no deseados en edificios y complejos residenciales, protegiendo a los residentes y sus bienes.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="4" img-src="https://www.homecenter.com.co/static/landing/guiasdecompra/Guias_de_compra_2/img/tipos-de-tornillos/tipos-de-tornillos-d.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Compra de articulos corporativos</div>
            <div class="text-subtitle1">Servicio de compras de miselanio, articulos con designacion número de parte o número de material, compras especializadas.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="3" img-src="https://i.ibb.co/z404q6W/aseo.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Administradora De Servicios Integrales</div>
            <div class="text-subtitle1">Somos profesionales en aseo y limpieza y buscamos entregar cada uno de nuestros servicios con atención de eficiencia y calidad enfocada en las necesidades de nuestros clientes.</div>
          </div>
        </q-carousel-slide>

        <q-carousel-slide :name="2" img-src="https://i.ibb.co/9yHtm62/aseo-profundo.jpg">
          <div class="absolute-bottom custom-caption">
            <div class="text-h2">Aseo 24 Hrs</div>
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
