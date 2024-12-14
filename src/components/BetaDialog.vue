<template>
    <v-dialog
      v-model="dialog"
      max-width="500"
    >
      <v-card class="pa-4">
        <v-card-title class="text-h5">
          ¡Conviértete en usuario beta!
        </v-card-title>
        <v-card-text>
          <p>Para convertirte en usuario beta, enviá un mail a rydiosupp@gmail.com con:</p>
          <ul>
            <li>Asunto: "Quiero ser usuario beta"</li>
            <li>Tu nombre completo</li>
          </ul>
          <v-alert
            type="info"
            class="mt-4"
            color="#59A58A"
          >
            Por el momento, la versión beta solo está disponible para dispositivos Android.
          </v-alert>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="#59A58A"
            dark
            class="custom-btn"
            @click="closeDialog"
          >
            cerrar
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </template>
  
  <script>
  export default {
    props: {
      value: Boolean
    },
    computed: {
      dialog: {
        get() {
          return this.value
        },
        set(value) {
          this.$emit('input', value)
        }
      }
    },
    methods: {
      closeDialog() {
        this.$emit('input', false)
      }
    }
  }
  </script>
  
  <style scoped>
  .custom-btn {
    border-radius: 28px !important;
    text-transform: none !important;
    letter-spacing: normal !important;
  }
  </style>