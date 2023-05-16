<template>
  <div ref="myListRef" class="row justify-right q-gutter-sm" style="margin-top: 80px;">
    <GoogleMap
      api-key="AIzaSyAHAiI5AUaZpLEHgg_3W32R2_ppYKP1SVc"
      style="width: 100%; height: 500px"
      :center="center"
      :zoom="17"
      >
        <Marker :options="{ position: center }" />
      </GoogleMap>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { GoogleMap, Marker } from 'vue3-google-map'

const center = ref({ lat: -33.4311736, lng: -70.6232534 })
</script>
  