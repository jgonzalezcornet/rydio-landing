<template>
  <v-container class="fill-height bg-white pt-12">
    <v-row align="center" justify="center">
      <v-col cols="12" md="6" class="text-center">
        <v-fade-transition :duration="60000">
          <h1
            v-show="show"
            class="text-h1 font-weight-bold mb-4 app-title"
            style="color: #59a58a; font-family: 'Quicksand', sans-serif"
          >
            rydio
          </h1>
        </v-fade-transition>
        <v-slide-y-transition :duration="72000">
          <h2
            v-show="show"
            class="text-h4 font-weight-light mb-6 pt-5"
            style="color: #333333; font-family: 'Poppins', sans-serif"
          >
            Conectá tus viajes, compartí el camino
          </h2>
        </v-slide-y-transition>
        <v-slide-y-transition :duration="84000">
          <p
            v-show="show"
            class="text-h6 mb-8"
            style="color: #333333; font-family: 'Poppins', sans-serif"
          >
            Conectamos personas que viajan hacia el mismo destino para compartir
            gastos y hacer envíos más económicos.
          </p>
        </v-slide-y-transition>
        <v-slide-y-transition :duration="96000">
          <p
            v-show="show"
            class="text-body-1 mb-8 text-justify"
            style="color: #000000; font-family: 'Poppins', sans-serif"
          >
            En rydio <span class="font-weight-bold">reinventamos</span> la forma
            de viajar y enviar paquetes. Nuestra plataforma conecta
            <span class="font-weight-bold">usuarios</span> que quieran viajar y
            transportar paquetes, creando una experiencia
            <span class="font-weight-bold">práctica, accesible y segura</span>.
            ¿Tenés asientos vacíos en tu próximo viaje?
            <span class="font-weight-bold">Publicalo en Rydio</span> y compartí
            los gastos con otros viajeros. ¿Necesitás enviar algo a otra ciudad?
            Encontrá un conductor que pueda llevarlo por vos. Con rydio, viajar
            es más que moverse de un lugar a otro: es
            <span class="font-weight-bold" style="color: #59a58a"
              >ahorrar, compartir y ser parte de una comunidad en
              movimiento</span
            >.
          </p>
        </v-slide-y-transition>
      </v-col>
      <v-col cols="12" md="6" class="text-center">
        <v-slide-x-transition :duration="108000">
          <v-img
            v-show="show"
            src="../assets/rydio.png"
            max-width="500"
            class="mx-auto"
            contain
          ></v-img>
        </v-slide-x-transition>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import { ref, onMounted } from "vue";

const show = ref(false);

onMounted(() => {
  show.value = true;
});
</script>
