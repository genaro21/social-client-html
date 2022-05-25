<template>
  <div class="rs-stats">
    <v-card dark class="card">
      <v-card-title class="rs-card-title">
        <v-icon size="32" class="mt-n4">mdi-chart-box</v-icon>
        <p class="headline mx-2">Stats</p>
      </v-card-title>
      <v-card-text class="rs-card-text">
        <v-list class="rs-list" light>
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-file-image</v-icon>
            </v-list-item-icon>
            <v-list-item-content>n# imagenes</v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-comment</v-icon>
            </v-list-item-icon>
            <v-list-item-content>n# comentarios</v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-thumb-up</v-icon>
            </v-list-item-icon>
            <v-list-item-content>n# views</v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-eye-settings</v-icon>
            </v-list-item-icon>
            <v-list-item-content>n# likes</v-list-item-content>
          </v-list-item>
        </v-list>
      </v-card-text>
    </v-card>
  </div>
</template>

<style scoped>
.rs-card-text {
  padding: 4px;
}

.rs-card-title {
  height: 60px;
}
.card {
  margin-bottom: 20px;
}
</style>
