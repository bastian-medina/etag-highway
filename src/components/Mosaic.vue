<template>
    <br><br>
    <div class="q-pa-md">
        <div class="row justify-center q-gutter-sm">
            <h4 class="q-display-2">Materiales y Compras especializadas</h4>
        </div>
      <div ref="myListRef" class="row justify-center q-gutter-sm">


        <q-intersection
          v-for="item, index in items"
          :key="index"
          :root="listEl"
          once
          transition="scale"
          class="col-2"
        >
            <q-card>
                <q-img :src="item.url" />
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
        url: "https://www.deskidea.com/blog/wp-content/uploads/2022/05/material-de-oficina.jpg",
    },
    {
        url: "https://media.istockphoto.com/id/1172864528/es/foto/bajo-el-sistema-de-filtro-de-agua-de-fregadero-en-un-hospital.jpg?s=612x612&w=0&k=20&c=wKp1fIWxiVsFB6ZCBulFhixTehHOqJBJInAGOu6DrJM=",
    },
    {
        url: "https://www.swagelok.com/-/media/blog/industrial-hose-replacement-core-tube-material-considerations/industrial-hose-banner.ashx?h=350&iar=0&w=700&hash=9EA25679AEB89AC444CD3368890B80FF",
    },
    {
        url: "https://www.rodamendez.cl/wp-content/uploads/2019/12/rodamientos-de-polines-cilindricos-1.jpg",
    },
    {
        url: "https://europer.cl/wp-content/uploads/2018/05/pernos.png",
    },
    {
        url: "https://www.deskidea.com/blog/wp-content/uploads/2022/06/material-oficina.jpg",
    },
    {
        url: "https://www.technoinjectiontools.mx/wp-content/uploads/2016/11/productos-limpieza-taller-mecanico.jpg",
    },
    {
        url: "https://steelprosafety.vteximg.com.br/arquivos/proteccion-manos-12.10.2021.jpg?v=637696467502300000",
    },
    {
        url: "https://www.kpnsafety.com/wp-content/uploads/2022/03/epp-para-seguridad-electrica2.jpeg",
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
  