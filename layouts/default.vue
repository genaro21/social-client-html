<template>
  <div class="rs-layout-default">
    <v-app>
      <RsAppBar />
      <v-main>
        <v-container>
          <v-row>
            <v-col cols="8">
              <Nuxt />
            </v-col>
            <v-col cols="4">
              <RsStats />
              <RsMostPopular />
              <RsLatestComments />
            </v-col>
          </v-row>
        </v-container>
      </v-main>
    </v-app>
  </div>
</template>
