<template>
  <div class="rs-sign-in-form">
    <v-row>
      <v-col cols="3"></v-col>
      <v-col cols="6">
        <v-card>
          <v-card-title>
            <div style="width: 100%; text-align: center">
              <p>Sign In</p>
            </div>
          </v-card-title>
          <v-card-text>
            <v-text-field placeholder="email" outlined></v-text-field>
            <v-text-field
              placeholder="password"
              type="password"
              outlined
            ></v-text-field>
            <v-btn color="success" block>Submit</v-btn>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="3"></v-col>
    </v-row>
  </div>
</template>
