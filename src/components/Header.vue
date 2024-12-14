<template>
    <v-app-bar
      app
      flat
      color="#59A58A"
      elevation="1"
      height="80"
    >
      <v-container class="py-0 fill-height d-flex align-center pl-0">
        <div class="text-h3 font-weight-bold white--text ml-2" style="font-family: 'Quicksand', sans-serif;">
          rydio
        </div>
        <v-spacer></v-spacer>
        <v-btn
          color="white"
          class="custom-btn mx-1"
          to="/Home"
        >
          Inicio
        </v-btn>
        <div class="divider"></div>
        <v-btn
          color="white" 
          class="custom-btn mx-1"
          to="/About"
        >
          Conocé al equipo
        </v-btn>
        <div class="divider"></div>
        <v-btn
          color="white"
          class="custom-btn mx-1 mr-2"
          to="/Download"
        >
          Descargá la app
        </v-btn>
      </v-container>
    </v-app-bar>
</template>

<style scoped>
.custom-btn {
  font-size: 1.1rem !important;
  border-radius: 28px !important;
  text-transform: none !important;
  letter-spacing: normal !important;
  transition: all 0.3s ease !important;
}

.custom-btn:hover {
  background-color: rgba(255, 255, 255, 0.2) !important;
  transform: scale(1.05);
}

.divider {
  height: 24px;
  width: 1px;
  background-color: white;
  opacity: 0.7;
  margin: 0 8px;
}
</style>