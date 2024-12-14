<template>
    <div>
      <v-btn
        x-large
        color="#59A58A"
        dark
        @click="dialog = true"
        class="custom-btn"
      >
        quiero ser usuario beta
      </v-btn>
      <BetaDialog
        v-model="dialog"
      />
    </div>
  </template>
  
  <script>
  import BetaDialog from './BetaDialog.vue'
  
  export default {
    components: {
      BetaDialog
    },
    data: () => ({
      dialog: false
    })
  }
  </script>
  
  <style scoped>
  .custom-btn {
    border-radius: 28px !important;
    text-transform: none !important;
    letter-spacing: normal !important;
  }
  </style>