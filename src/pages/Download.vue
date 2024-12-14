<template>
  <div>
    <v-container class="mt-16 pa-0 fill-width" fluid>
      <v-row justify="center">
        <v-col cols="12" class="text-center mb-16">
          <h1 class="text-h2 font-weight-bold" style="font-family: 'Poppins', sans-serif;">Descargá <span class="font-weight-bold" style="color: #59A58A; font-family: 'Quicksand', sans-serif;">rydio</span></h1>
        </v-col>
      </v-row>

      <v-row justify="center" class="mb-16">
        <v-col cols="12" md="5">
          <v-card
            class="pa-8 rounded-xl h-100"
            elevation="2"
            style="background: linear-gradient(145deg, #ffffff, #f5f5f5)"
          >
            <h2 class="text-h4 mb-6 font-weight-medium" style="color: #333333; font-family: 'Poppins', sans-serif;">Estado actual</h2>
            <p class="text-body-1 mb-6" style="color: #333333; font-family: 'Poppins', sans-serif;">
              Actualmente, rydio se encuentra en <span style="color: #59A58A" class="font-weight-bold">fase beta</span> y está disponible exclusivamente para usuarios seleccionados, únicamente en dispositivos Android.
            </p>
            <p class="text-subtitle-1 mb-6" style="color: #333333; font-family: 'Poppins', sans-serif;">
              Próximamente la aplicación estará disponible para todos los usuarios, a un solo click desde tu celular. </p>
            <div class="d-flex justify-center">
              <v-chip
                class="mx-2 pa-6"
                disabled
                size="x-large"
                variant="elevated"
                style="background-color: #f5f5f5; border: 1px solid #e0e0e0"
              >
                <v-icon size="32" class="mr-2" color="#000000">mdi-google-play</v-icon>
                <span style="color: #000000; font-family: 'Poppins', sans-serif; font-size: 1.1rem">Play Store</span>
              </v-chip>
              <v-chip
                class="mx-2 pa-6"
                disabled
                size="x-large"
                variant="elevated"
                style="background-color: #f5f5f5; border: 1px solid #e0e0e0"
              >
                <v-icon size="32" class="mr-2" color="#666666">mdi-apple</v-icon>
                <span style="color: #111111; font-family: 'Poppins', sans-serif; font-size: 1.1rem">App Store</span>
              </v-chip>
            </div>
          </v-card>
        </v-col>

        <v-col cols="12" md="5">
          <v-card
            class="pa-8 rounded-xl h-100"
            elevation="2"
            style="background: linear-gradient(145deg, #ffffff, #f5f5f5)"
          >
            <h2 class="text-h4 mb-6 font-weight-medium" style="color: #333333; font-family: 'Poppins', sans-serif;">¿Querés ser usuario beta?</h2>
            <p class="text-body-1 mb-6" style="color: #333333; font-family: 'Poppins', sans-serif;">
              Para convertirte en usuario beta, enviá un mail a:
            </p>
            <v-btn
              block
              color="#59A58A"
              class="mb-6 py-6 text-body-1 custom-btn"
              rounded="xl"
              variant="flat"
              @click="sendEmail"
              style="font-family: 'Poppins', sans-serif;"
            >
              rydiosupp@gmail.com
            </v-btn>
            <p class="text-body-1 mb-2" style="color: #333333; font-family: 'Poppins', sans-serif;">
              Incluí la siguiente información:
            </p>
            <v-list class="bg-transparent" density="compact">
              <v-list-item>
                <template v-slot:prepend>
                  <v-icon color="#59A58A">mdi-email-outline</v-icon>
                </template>
                <v-list-item-title style="color: #333333; font-family: 'Poppins', sans-serif;">Asunto: "Usuario beta"</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <template v-slot:prepend>
                  <v-icon color="#59A58A">mdi-account-outline</v-icon>
                </template>
                <v-list-item-title style="color: #333333; font-family: 'Poppins', sans-serif;">Tu nombre completo</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <template v-slot:prepend>
                  <v-icon color="#59A58A">mdi-text-box-outline</v-icon>
                </template>
                <v-list-item-title class="overflow-visible" style="color: #333333; font-family: 'Poppins', sans-serif;">
                  Contanos por qué querés ser usuario beta
                </v-list-item-title>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup>
const sendEmail = () => {
  window.location.href = 'mailto:rydiosupp@gmail.com'
}
</script>

<style scoped>
.custom-btn {
  border-radius: 28px !important;
  text-transform: none !important;
  letter-spacing: normal !important;
  transition: all 0.3s ease !important;
}

.custom-btn:hover {
  transform: scale(1.05);
}

.v-card {
  transition: transform 0.3s ease;
}

.v-card:hover {
  transform: scale(1.02);
}
</style>