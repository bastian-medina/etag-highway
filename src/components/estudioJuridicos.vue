<template>
    <br><br>
    <div class="q-pa-md">
        <div class="row justify-center q-gutter-sm">
            <h4 class="q-display-2">Tipos de Servicios</h4>
        </div>
      <div ref="myListRef" class="row justify-center q-gutter-sm">


        <q-intersection
          v-for="item, index in items"
          :key="index"
          :root="listEl"
          once
          transition="scale"
          class="col-md-3 .col-md-auto"
        >
            <q-card class="q-ma-sm">
                <q-img :src="item.url" />

                <q-card-section>
                    <div class="fontsize-12 text-weight-bold">{{ item.titleCard }}</div>
                    <div class="text-caption text-grey">{{ item.informationCard }}</div>
                </q-card-section>

                <q-card-actions vertical align="center">
                    <q-btn push style="background-color: #c86b85;" text-color="white" :label="item.buttonCard" />
                </q-card-actions>
            </q-card>
        </q-intersection>
      </div>
    </div>
</template>
  
<script setup>
import { ref, computed } from 'vue'
  
const myListRef = ref(null)
const items = ref([
    {
        url: "https://mantiene.cl/assets/img/projects/1.jpg",
        titleCard: " ASEO PREVENTIVO",
        informationCard: "Prestamos un servicio de visitas y mantenciones programadas a recintos comerciales para evitar la problemática que emana del desgaste natural de los bienes mobiliarios del cliente.",
        buttonCard: "Ver más"
    },
    {
        url: "https://mantiene.cl/assets/img/projects/2.jpg",
        titleCard: "ASEO REACTIVO",
        informationCard: "Prestamos un servicio de visitas y mantenciones programadas a recintos comerciales para evitar la problemática que emana del desgaste natural de los bienes mobiliarios del cliente.",
        buttonCard: "Ver más"
    },
    {
        url: "https://mantiene.cl/assets/img/projects/5.jpg",
        titleCard: "ASEO 24 Hrs",
        informationCard: "Prestamos un servicio de visitas y mantenciones programadas a recintos comerciales para evitar la problemática que emana del desgaste natural de los bienes mobiliarios del cliente.",
        buttonCard: "Ver más"
    },
    {
        url: "https://equipamientoyseguridad.com/wp-content/uploads/instalacion-camaras-de-vigilancia-negocio.jpg",
        titleCard: "Servicios de vigilancia",
        informationCard: "Ofrecemos servicios de vigilancia y mantenimiento programado a recintos comerciales para garantizar la seguridad y prevenir posibles daños en los bienes mobiliarios del cliente debido al desgaste natural.",
        buttonCard: "Ver más"
    },
    {
        url: "https://cleancontrol.es/wp-content/uploads/2021/02/conserjeria-min-1024x589.jpg",
        titleCard: "Servicios de conserjería",
        informationCard: "Ofrecemos servicios de conserjería personalizados para edificios y complejos residenciales, incluyendo gestión de acceso, recepción de paquetes y mantenimiento de áreas comunes. Disponibles las 24 horas del día.",
        buttonCard: "Ver más"
    },
    {
        url: "https://mantiene.cl/assets/img/projects/3.jpg",
        titleCard: "Proyectos electricos y adicionales",
        informationCard: "Prestamos un servicio de visitas, mantenciones y proyectos electricos programadas a recintos comerciales para evitar futuras problemáticas.",
        buttonCard: "Ver más"
    },
    {
        url: "https://www.lyms.net/wp-content/uploads/2016/01/limpieza-oficinas-Zaragoza.jpg",
        titleCard: "Aseo de oficinas",
        informationCard: "Los servicios de oficina proporcionan soluciones profesionales y eficientes para la gestión de tareas administrativas y el mantenimiento de un espacio de trabajo productivo y organizado.",
        buttonCard: "Ver más"
    },
])
const listEl = computed(() => myListRef.value ? myListRef.value.$el : null)

</script>
  
  <style scoped>
  .example-item {
    height: 290px;
    width: 290px;
  }
  </style>
  