<template>
  <div>
    <v-container class="fill-height fill-width pb-6">
      <v-row justify="center" align="center" class="mt-16">
        <v-col cols="12">
          <v-row justify="center">
            <v-col cols="12" sm="4" class="text-center">
              <v-avatar size="200" class="mb-4 avatar-hover">
                <v-img src="../assets/conra.jpeg" cover></v-img>
              </v-avatar>
              <h3
                class="text-h5 font-weight-bold name-hover"
                style="font-family: 'Poppins', sans-serif"
              >
                Conrado Hillar
              </h3>
            </v-col>

            <v-col cols="12" sm="4" class="text-center">
              <v-avatar size="200" class="mb-4 avatar-hover">
                <v-img src="../assets/eze.jpeg" cover></v-img>
              </v-avatar>
              <h3
                class="text-h5 font-weight-bold name-hover"
                style="font-family: 'Poppins', sans-serif"
              >
                Ezequiel Testoni
              </h3>
            </v-col>

            <v-col cols="12" sm="4" class="text-center">
              <v-avatar size="200" class="mb-4 avatar-hover">
                <v-img src="../assets/santi.jpeg" cover></v-img>
              </v-avatar>
              <h3
                class="text-h5 font-weight-bold name-hover"
                style="font-family: 'Poppins', sans-serif"
              >
                Santiago Bassi
              </h3>
            </v-col>
          </v-row>
        </v-col>

        <v-col cols="12">
          <v-row justify="center">
            <v-col cols="12" sm="4" class="text-center">
              <v-avatar size="200" class="mb-4 avatar-hover">
                <v-img src="../assets/i.jpeg" cover></v-img>
              </v-avatar>
              <h3
                class="text-h5 font-weight-bold name-hover"
                style="font-family: 'Poppins', sans-serif"
              >
                Ignacio Maruottolo
              </h3>
            </v-col>

            <v-col cols="12" sm="4" class="text-center">
              <v-avatar size="200" class="mb-4 avatar-hover">
                <v-img src="../assets/jose.jpeg" cover></v-img>
              </v-avatar>
              <h3
                class="text-h5 font-weight-bold name-hover"
                style="font-family: 'Poppins', sans-serif"
              >
                Josefina Gonzalez Cornet
              </h3>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <v-container
      class="mt-12 rounded-xl py-8"
      style="background-color: #59a58a"
    >
      <v-row align="center" justify="center">
        <v-col cols="12" md="8" class="text-center">
          <v-scale-transition>
            <p
              v-show="show"
              class="text-h5 font-weight-regular text-white"
              style="line-height: 1.8; font-family: 'Poppins', sans-serif"
            >
              Somos un grupo de estudiantes de Ingeniería Informática del ITBA,
              unidos por nuestra pasión por la tecnología y la innovación. Lo
              que comenzó como un proyecto académico se transformó en
              <span class="font-weight-bold">rydio</span>, un servicio de car
              sharing y envío de paquetes que busca facilitar la movilidad
              urbana en Argentina. En rydio, nos dedicamos a crear soluciones
              inteligentes que mejoren la experiencia de quienes necesitan
              moverse o enviar un paquete de forma rápida y segura. Desde la
              programación hasta el diseño de la plataforma, cada miembro del
              equipo aporta su expertise para hacer de rydio una herramienta más
              eficiente, accesible y sostenible para todos.
            </p>
          </v-scale-transition>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const show = ref(false);

onMounted(() => {
  show.value = true;
});
</script>

<style scoped>
.avatar-hover {
  transition: transform 0.4s ease;
}

.avatar-hover:hover {
  transform: scale(1.1);
}

.name-hover {
  transition: transform 0.3s ease;
}

.col:hover .name-hover {
  transform: scale(1.1);
}
</style>
