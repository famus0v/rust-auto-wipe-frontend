<template>
    <v-container  class="d-flex align-center justify-center" >
      <v-card height="400px" width="800px" variant="tonal" class="pa-4">
        <v-row>
          <!-- Аватарка -->
          <v-col cols="auto">
            <v-avatar size="200px">
              <v-img
                alt="Avatar"
                src="https://lastfm.freetls.fastly.net/i/u/ar0/c099708e97fc42c9c29dbcbcd82684ff.png"
              />
            </v-avatar>
            <div class="text-center mt-4 text-md-h5">22:06:31</div>
          </v-col>
          <v-col>
            <v-row>
              <v-card-title class="text-lg-h4">Nickname</v-card-title>
              <div class="balance-text text-h6">202<v-icon>mdi-currency-rub</v-icon></div>
            </v-row>
            <div class="mt-4">Servers:</div>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </template>
  
  <style scoped>
    .balance-text {
    position: absolute;
    top: 16px; 
    right: 10px; 
    font-weight: bold;
}

</style>
  <script setup>
    //
  </script>
  