<template>
  <q-footer reveal bordered style="background-color: #cfd5e1;" class="text-black">
    <q-toolbar style="background-color: #cfd5e1;" class="text-black">
      
      <q-btn-dropdown stretch flat label="Contactos" class="mobile-hide">
        <q-list>


          <q-item-label header>Correo</q-item-label>
          <q-item clickable v-close-popup tabindex="0">
            <q-item-section avatar>
              <q-avatar icon="email" text-color="black" />
            </q-item-section>
            <q-item-section>
              <q-item-label>Correo principal</q-item-label>
              <q-item-label caption>etag@servicios.cl</q-item-label>
            </q-item-section>
          </q-item>
          <q-separator  />


          <q-item-label header>Redes Sociales</q-item-label>
          <q-item clickable v-close-popup tabindex="0">
            <q-item-section>
              <q-avatar icon="facebook" color="primary" text-color="white" />
            </q-item-section>
            <q-item-section>
              <q-item-label class="text-black">Facebook</q-item-label>
              <q-item-label caption>etag</q-item-label>
            </q-item-section>
          </q-item>

        </q-list>
      </q-btn-dropdown>

      <q-space />

      <q-list dark separator style="max-width: 318px" class="mobile-hide">
        <q-item v-ripple>
          <q-item-section>
            <q-item-label class="text-black">Horarios de atención:</q-item-label>
            <q-item-label  class="text-black" caption>- 9:00 a 13:00 Hrs</q-item-label>
            <q-item-label  class="text-black" caption>- 15:00 a 18:00 Hrs</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>

      <q-space/>
      <q-list dark separator style="max-width: 318px" class="mobile-hide">
        <q-item v-ripple>
          <q-item-section>
            <q-item-label  class="text-black">Dirección:</q-item-label>
            <q-item-label caption  class="text-black">Of. 403, piso 4, calle Huelen N°10, Providencia</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
      <q-space/>
      <q-list dark separator style="max-width: 318px">
        <q-item v-ripple>
          <q-item-section>
            <q-item-label caption class="text-black">© Servicos en Santiago | Desarrollado por BM</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>

    </q-toolbar>
</q-footer>
</template>

<style>
.text-black {
  color: #000000;
}
</style>