<template>
  <div class="rs-card">
    <v-card class="card">
      <v-card-title
        v-if="header"
        :class="remove ? 'rs-card-title rs-remove' : 'rs-card-title rs-black'"
      >
        <div class="rs-card-remove d-flex justify-space-between" v-if="remove">
          <p class="headline mx-2 white--text">{{ title }}</p>
          <v-btn color="error">Delete</v-btn>
        </div>
        <div class="d-flex justify-start" v-else>
          <v-icon color="white" size="32" class="mt-n4">{{ icon }}</v-icon>
          <p class="headline mx-2 white--text">{{ title }}</p>
        </div>
      </v-card-title>
      <v-card-text class="rs-card-text">
        <div class="rs-card-text-container">
          <slot />
        </div>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
    },
    icon: {
      type: String,
      default: undefined,
    },
    remove: {
      type: Boolean,
      default: false,
    },
    header: {
      type: Boolean,
      default: true,
    },
  },
}
</script>

<style scoped>
.rs-black {
  background-color: rgb(39, 39, 39);
}
.rs-remove {
  background-color: rgb(185, 38, 107);
}
.rs-card-text {
  background-color: white;
  border: rgb(39, 39, 39) 4px solid;
}

.rs-card-title {
  height: 60px;
}
.card {
  margin-bottom: 20px;
}
.texto {
  color: black;
}
.rs-card-text-container {
  padding-top: 20px;
}
.rs-card-remove {
  width: 100%;
}
</style>
